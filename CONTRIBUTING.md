# Contributing to Portal IQ

Thank you for your interest in contributing to Portal IQ! We welcome contributions from the community to help improve developer portal assessments and platform engineering practices.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Getting Started](#getting-started)
- [Development Process](#development-process)
- [Submitting Contributions](#submitting-contributions)
- [Style Guidelines](#style-guidelines)
- [Testing Requirements](#testing-requirements)
- [Documentation](#documentation)
- [Community](#community)

---

## Code of Conduct

This project adheres to a Code of Conduct that all contributors are expected to follow. By participating, you agree to maintain a respectful, inclusive, and professional environment.

### Our Standards

- **Be respectful** of differing viewpoints and experiences
- **Be collaborative** and constructive in feedback
- **Focus on what's best** for the community and the project
- **Show empathy** towards other community members
- **Be professional** in all interactions

### Unacceptable Behavior

- Harassment, discrimination, or personal attacks
- Trolling, insulting comments, or political arguments
- Publishing others' private information
- Other conduct inappropriate in a professional setting

Report violations to: conduct@platformetrics.com

---

## How Can I Contribute?

### 🐛 Reporting Bugs

Before creating a bug report, please check existing issues to avoid duplicates.

**Good bug reports include:**

- Clear, descriptive title
- Detailed steps to reproduce
- Expected vs. actual behavior
- Screenshots or error messages (if applicable)
- Environment details (OS, browser, tool version)
- Sample assessment data (anonymized)

**Template:**
````markdown
**Describe the bug**
A clear description of what the bug is.

**To Reproduce**
Steps to reproduce:
1. Go to '...'
2. Click on '...'
3. Enter data '...'
4. See error

**Expected behavior**
What you expected to happen.

**Screenshots**
If applicable, add screenshots.

**Environment:**
 - OS: [e.g., macOS 14.0]
 - Browser: [e.g., Chrome 119]
 - Version: [e.g., 1.0.0]

**Additional context**
Any other relevant information.
````

### 💡 Suggesting Enhancements

Enhancement suggestions are welcome! Please provide:

- Clear use case and rationale
- Expected behavior and benefits
- Implementation considerations (if known)
- Impact on existing functionality

### 📊 Contributing Assessment Data

Help improve Portal IQ's benchmark accuracy by contributing anonymized assessment data.

**Requirements:**
- Data must be anonymized (no company/personal identifiers)
- Include consent for research use
- Provide context (industry, org size, portal type)

**Process:**
1. Contact data@platformetrics.com
2. Sign data contribution agreement
3. Submit data via secure transfer
4. Receive aggregated insights in return

### 📝 Improving Documentation

Documentation improvements are highly valued:

- Fix typos, grammar, or clarity issues
- Add examples or use cases
- Improve API documentation
- Translate content (contact us first)
- Write tutorials or guides

### 🔬 Research Contributions

Contribute to Portal IQ's methodology:

- Validate scoring algorithms
- Propose new dimensions or metrics
- Share empirical studies
- Suggest statistical improvements

### 💻 Code Contributions

See [Development Process](#development-process) below.

---

## Getting Started

### Prerequisites

- **Python 3.9+**
- **Git**
- **Virtual environment tool** (venv, conda, etc.)
- **Basic understanding** of statistics and web development

### Fork and Clone

1. Fork the repository on GitHub
2. Clone your fork locally:
````bash
git clone https://github.com/YOUR-USERNAME/platformetrics-portal-iq.git
cd platformetrics-portal-iq
````

3. Add upstream remote:
````bash
git remote add upstream https://github.com/achankra/platformetrics-portal-iq.git
````

### Development Setup

1. Create a virtual environment:
````bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
````

2. Install dependencies:
````bash
pip install -r requirements.txt
pip install -r requirements-dev.txt  # Development dependencies
````

3. Install pre-commit hooks:
````bash
pre-commit install
````

4. Verify setup:
````bash
pytest tests/
````

### Project Structure
````
platformetrics-portal-iq/
├── src/
│   ├── assessment/        # Core assessment logic
│   ├── scoring/          # Scoring algorithms
│   ├── benchmarks/       # Benchmark data and normalization
│   ├── models/           # Statistical models
│   └── utils/            # Utility functions
├── tests/
│   ├── unit/             # Unit tests
│   ├── integration/      # Integration tests
│   └── fixtures/         # Test data
├── docs/                 # Documentation
├── examples/             # Example assessments
└── scripts/              # Utility scripts
````

---

## Development Process

### Branching Strategy

- **main**: Production-ready code
- **develop**: Integration branch for features
- **feature/**: New features (`feature/add-new-dimension`)
- **bugfix/**: Bug fixes (`bugfix/scoring-calculation`)
- **docs/**: Documentation updates (`docs/update-readme`)

### Workflow

1. **Sync with upstream:**
````bash
git checkout develop
git pull upstream develop
````

2. **Create a feature branch:**
````bash
git checkout -b feature/your-feature-name
````

3. **Make your changes:**
   - Write clean, documented code
   - Follow style guidelines
   - Add tests for new functionality
   - Update documentation

4. **Commit your changes:**
````bash
git add .
git commit -m "feat: add new capability dimension"
````

**Commit message format:**
- `feat:` New feature
- `fix:` Bug fix
- `docs:` Documentation changes
- `test:` Test additions/changes
- `refactor:` Code refactoring
- `perf:` Performance improvements
- `chore:` Maintenance tasks

5. **Keep your branch updated:**
````bash
git fetch upstream
git rebase upstream/develop
````

6. **Push to your fork:**
````bash
git push origin feature/your-feature-name
````

7. **Open a Pull Request** (see [Submitting Contributions](#submitting-contributions))

---

## Submitting Contributions

### Pull Request Process

1. **Before submitting:**
   - Ensure all tests pass: `pytest tests/`
   - Run linting: `flake8 src/`
   - Check formatting: `black --check src/`
   - Update documentation if needed
   - Verify no merge conflicts

2. **PR Description should include:**
   - Summary of changes
   - Motivation and context
   - Related issue numbers (`Fixes #123`)
   - Testing performed
   - Screenshots (for UI changes)
   - Breaking changes (if any)

3. **PR Template:**
````markdown
## Description
Brief description of changes.

## Motivation
Why is this change necessary?

## Type of Change
- [ ] Bug fix (non-breaking)
- [ ] New feature (non-breaking)
- [ ] Breaking change
- [ ] Documentation update

## Testing
How was this tested?

## Checklist
- [ ] Tests pass locally
- [ ] Code follows style guidelines
- [ ] Documentation updated
- [ ] No breaking changes (or documented)
- [ ] Commit messages follow convention
````

4. **Review Process:**
   - Maintainers will review within 5 business days
   - Address feedback promptly
   - Squash commits if requested
   - Be responsive to questions

5. **After Approval:**
   - Maintainer will merge
   - Delete your feature branch
   - Celebrate! 🎉

---

## Style Guidelines

### Python Code Style

Follow **PEP 8** with these specifics:

- **Line length:** 100 characters
- **Indentation:** 4 spaces
- **Quotes:** Double quotes for strings
- **Imports:** Organized (stdlib, third-party, local)

**Use Black for formatting:**
````bash
black src/ tests/
````

**Use Flake8 for linting:**
````bash
flake8 src/ tests/
````

### Code Quality Standards

- **Functions:** Single responsibility, < 50 lines
- **Classes:** Clear purpose, < 300 lines
- **Modules:** Cohesive functionality
- **Comments:** Explain "why", not "what"
- **Docstrings:** All public functions/classes

**Docstring format (Google style):**
````python
def calculate_dimension_score(capabilities, weights):
    """Calculate aggregated dimension score using weighted harmonic mean.
    
    Args:
        capabilities (list): List of capability scores [0, 1].
        weights (list): List of weights corresponding to capabilities.
        
    Returns:
        float: Dimension score [0, 1].
        
    Raises:
        ValueError: If lengths don't match or weights don't sum to 1.
        
    Example:
        >>> calculate_dimension_score([0.8, 0.6, 0.9], [0.3, 0.4, 0.3])
        0.73
    """
    # Implementation
````

### Statistical Code Guidelines

- **Use established libraries:** NumPy, SciPy, scikit-learn
- **Document assumptions:** Clearly state statistical assumptions
- **Provide references:** Cite methodology sources
- **Validate numerically:** Check edge cases and stability
- **Handle uncertainty:** Report confidence intervals where appropriate

---

## Testing Requirements

### Test Coverage

- **Minimum coverage:** 80%
- **Critical paths:** 100% coverage
- **New features:** Must include tests

**Check coverage:**
````bash
pytest --cov=src --cov-report=html tests/
````

### Types of Tests

**Unit Tests:**
- Test individual functions
- Mock external dependencies
- Fast execution (< 0.1s each)
````python
def test_harmonic_mean_calculation():
    """Test weighted harmonic mean with known values."""
    scores = [0.8, 0.6, 0.9]
    weights = [1/3, 1/3, 1/3]
    expected = 0.73
    result = calculate_harmonic_mean(scores, weights)
    assert abs(result - expected) < 0.01
````

**Integration Tests:**
- Test component interactions
- Use realistic data
- Verify end-to-end workflows

**Statistical Tests:**
- Validate against known distributions
- Test edge cases (zeros, ones, NaN)
- Verify mathematical properties

### Test Data

- Use fixtures in `tests/fixtures/`
- Anonymize any real data
- Document test data sources

---

## Documentation

### Documentation Requirements

**For all contributions:**
- Update relevant docs in `docs/`
- Add docstrings to new code
- Update CHANGELOG.md
- Include inline comments for complex logic

**For new features:**
- Add usage examples
- Update API documentation
- Include methodology explanation (if applicable)
- Update README.md if user-facing

### Documentation Style

- **Clear and concise:** Avoid jargon where possible
- **Examples:** Include practical examples
- **Structure:** Use headers, lists, and tables
- **Links:** Reference related documentation
- **Diagrams:** Use Mermaid for flowcharts/diagrams

**Example:**
````markdown
## Feature: New Dimension Assessment

### Overview
Brief description of the feature.

### Usage
```python
from src.assessment import assess_dimension

result = assess_dimension(
    capability_scores=[0.7, 0.8, 0.6],
    dimension="automation"
)
print(result.score)  # 0.70
```

### Methodology
Explanation of how this works, including:
- Statistical approach
- Assumptions
- Limitations

### See Also
- [Related Feature](link)
- [Theory Documentation](link)
````

---

## Community

### Getting Help

- **GitHub Issues:** Technical questions and bugs
- **GitHub Discussions:** General questions and ideas
- **Email:** support@platformetrics.com for private inquiries

### Recognition

Contributors are recognized in:
- CONTRIBUTORS.md
- Release notes
- Annual contributor highlights

### Communication Channels

- **GitHub:** Primary communication
- **LinkedIn:** [Platformetrics Company Page](https://linkedin.com/company/platformetrics)
- **Website:** [www.platformetrics.com](https://www.platformetrics.com)

---

## License

By contributing to Portal IQ, you agree that your contributions will be licensed under the same license as the project. See [LICENSE](LICENSE) for details.

For proprietary contributions or alternative licensing, contact: legal@platformetrics.com

---

## Questions?

Don't hesitate to ask! We're here to help:

- Open a [GitHub Discussion](https://github.com/achankra/platformetrics-portal-iq/discussions)
- Email: contributors@platformetrics.com
- Review existing [documentation](docs/)

---

## Thank You!

Your contributions make Portal IQ better for everyone. We appreciate your time and effort in helping improve developer portal assessments and platform engineering practices.

**Happy contributing!** 🚀

---

*Last updated: November 2025*
