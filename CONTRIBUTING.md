# Contributing to MegaBasket E-Commerce Platform

First off, thank you for considering contributing to **MegaBasket**! It's people like you that make MegaBasket such a robust and modern platform.

All kinds of contributions are welcome: bug fixes, feature additions, performance optimizations, documentation enhancements, UI/UX polish, and suggestions.

---

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
  - [Reporting Bugs](#reporting-bugs)
  - [Suggesting Enhancements](#suggesting-enhancements)
  - [Pull Requests](#pull-requests)
- [Development Setup](#development-setup)
  - [Prerequisites](#prerequisites)
  - [Fork & Clone](#fork--clone)
  - [Backend Setup](#backend-setup)
  - [Frontend Setup](#frontend-setup)
  - [ML Service Setup (Optional)](#ml-service-setup-optional)
- [Coding Guidelines](#coding-guidelines)
  - [Commit Message Format](#commit-message-format)
  - [Code Style & Best Practices](#code-style--best-practices)
- [Contact & Support](#contact--support)

---

## Code of Conduct

This project and everyone participating in it is governed by the [MegaBasket Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to [megabasket.v01@gmail.com](mailto:megabasket.v01@gmail.com).

---

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check existing [Issues](https://github.com/Saurabhtbj1201/MegaBasket-E-commerce-Platform/issues) to make sure it hasn't already been reported.

When creating a bug report, please include as much detail as possible:
- **Title**: A clear and descriptive title.
- **Description**: Detailed description of the bug and how it occurred.
- **Steps to Reproduce**: Step-by-step instructions.
- **Expected vs Actual Behavior**: What should happen vs what actually happened.
- **Screenshots or Logs**: Console errors or UI screenshots.
- **Environment**: OS version, browser version, Node.js version.

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues.
- Use a clear and descriptive title.
- Provide a step-by-step description of the suggested feature or enhancement.
- Explain why this enhancement would be useful to most MegaBasket users.
- Add mockup images or wireframes if applicable.

### Pull Requests

1. **Fork the repository** on GitHub.
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/<your-username>/MegaBasket-E-commerce-Platform.git
   cd MegaBasket-E-commerce-Platform
   ```
3. **Create a new branch** for your feature or bug fix:
   ```bash
   git checkout -b feature/amazing-feature
   # or
   git checkout -b fix/bug-description
   ```
4. **Make your changes**, keeping them focused on a single concern.
5. **Test thoroughly**: Ensure both frontend and backend work without errors.
6. **Commit your changes** with descriptive commit messages following Conventional Commits.
7. **Push to your fork**:
   ```bash
   git push origin feature/amazing-feature
   ```
8. **Open a Pull Request** against the `master` branch of the upstream repository.

---

## Development Setup

### Prerequisites

- **Node.js**: v18.x or v20.x+
- **npm** or **yarn**
- **Python**: 3.9+ (if working on the ML recommendation service)
- **MongoDB**: Local MongoDB instance or free [MongoDB Atlas](https://www.mongodb.com/atlas) cluster
- **Git**

### Fork & Clone

```bash
git clone https://github.com/Saurabhtbj1201/MegaBasket-E-commerce-Platform.git
cd MegaBasket-E-commerce-Platform
```

### Backend Setup

```bash
cd backend
npm install
cp .env.example .env # Update with your database & secret credentials
npm run dev
```
The backend server runs at `http://localhost:5000`.

### Frontend Setup

```bash
cd ../frontend
npm install
npm run dev
```
The frontend Vite server runs at `http://localhost:5173`.

### ML Service Setup (Optional)

```bash
cd ../ml-service
python -m venv venv
# Windows:
.\venv\Scripts\activate
# Linux/macOS:
source venv/bin/activate

pip install -r requirements.txt
python app.py
```
The ML microservice runs at `http://localhost:5001`.

---

## Coding Guidelines

### Commit Message Format

We adhere to the [Conventional Commits](https://www.conventionalcommits.org/) specification:

- `feat:` A new feature
- `fix:` A bug fix
- `docs:` Documentation only changes
- `style:` Formatting changes that do not affect code logic (white-space, formatting, etc.)
- `refactor:` A code change that neither fixes a bug nor adds a feature
- `perf:` A code change that improves performance
- `test:` Adding missing tests or correcting existing tests
- `chore:` Changes to the build process or auxiliary tools and libraries

*Example:* `feat(auth): add Google OAuth login integration`

### Code Style & Best Practices

- Keep code clean, modular, and well-commented.
- Preserve consistent formatting and avoid unused imports.
- Never commit sensitive keys, passwords, or personal tokens (`.env` files must stay ignored).
- Write self-explanatory variable and function names.

---

## Contact & Support

If you have questions or need assistance with your contribution:
- **Email**: [megabasket.v01@gmail.com](mailto:megabasket.v01@gmail.com)
- **GitHub Discussions / Issues**: [Open an issue](https://github.com/Saurabhtbj1201/MegaBasket-E-commerce-Platform/issues)
- **Developer**: [Saurabh Kumar](https://github.com/Saurabhtbj1201)

Thank you for contributing to MegaBasket! 🛒✨
