# robotics-rigid-body-mechanics

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) [![Release](https://img.shields.io/github/v/release/wuji-technology/robotics-rigid-body-mechanics)](https://github.com/wuji-technology/robotics-rigid-body-mechanics/releases)

Lecture notes on robotics rigid body mechanics. LaTeX document covering core theories of rigid body motion and dynamics in robotics, including rotation, screw theory, dynamics, and multibody systems.

## Table of Contents

- [Repository Structure](#repository-structure)
- [Usage](#usage)
- [Contact](#contact)

## Repository Structure

```text
├── images/
├── sections/
│   ├── cover.tex
│   ├── foreword.tex
│   ├── intro.tex
│   ├── rotation.tex
│   ├── screw.tex
│   ├── dynamics.tex
│   └── multibody.tex
├── main.tex
└── README.md
```

### Directory Description

| Directory | Description |
|-----------|-------------|
| `images/` | Image resources for the document |
| `sections/` | Chapter content files including cover, foreword, introduction, rotation, screw theory, dynamics, and multibody systems |
| `main.tex` | Main LaTeX document entry point |

## Usage

### Prerequisites

- TeX distribution (TeX Live or MiKTeX)

**Ubuntu/Debian:**

```bash
sudo apt install texlive-xetex texlive-lang-chinese texlive-lang-greek texlive-latex-extra texlive-science texlive-pictures
```

**macOS (Homebrew):**

```bash
brew install --cask basictex
sudo tlmgr update --self
sudo tlmgr install ctex standalone mathtools textgreek greek-fontenc fancyhdr footmisc enumitem cbfonts
```

### Running

Compile with `xelatex` (run twice to generate table of contents):

```bash
xelatex main.tex
xelatex main.tex
```

Or use `latexmk` for automatic multi-pass compilation:

```bash
latexmk -xelatex main.tex
```

### Output

Successful compilation generates `main.pdf`.

## Contact

For any questions, please contact support@wuji.tech.
