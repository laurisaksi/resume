# Resume of Lauri Saksi

[Finnish version](https://laurisaksi.github.io/resume/)

[English version](https://registry.jsonresume.org/laurisaksi?theme=even)

## 🌟 Overview

This repository contains a professional resume system that automatically generates and deploys resumes in multiple languages (Finnish and English) with different themes. The system uses JSON Resume standards and includes automated CI/CD pipelines.

## 📁 Repository Structure

```
resume/
├── .github/workflows/          # CI/CD automation
│   ├── deploy-fi-resume.yml    # Finnish resume deployment
│   └── gist.yml               # Gist update automation
├── en/                         # English resume
│   ├── resume.json            # English resume data
│   └── index.html             # Generated HTML (deployed)
├── fi/                         # Finnish resume
    ├── resume.json            # Finnish resume data
    └── index.html             # Generated HTML (deployed)

```

## 🛠️ Technology Stack

- **Core**: JSON Resume standard
- **Themes**:
  - `jsonresume-theme-elegant` (English)
  - `jsonresume-theme-even` (Finnish)
- **Build Tool**: `resumed` CLI
- **PDF Generation**: Puppeteer
- **Quality Tools**: Prettier, Husky, lint-staged
- **Deployment**: GitHub Actions, GitHub Pages

## 📝 Available Scripts

#### Resume Generation

```bash
# Generate HTML versions
npm run html-fi      # Finnish resume HTML
npm run html-en      # English resume HTML

# Generate PDF versions
npm run pdf-fi       # Finnish resume PDF
npm run pdf-en       # English resume PDF
```

#### Validation

```bash
# Validate resume JSON files
npm run validate-fi  # Finnish resume validation
npm run validate-en  # English resume validation
```

#### Code Quality

```bash
# Check code formatting
npm run lint

# Fix formatting issues
npm run lint:fix
```

## 🔄 Automated Workflows

### Finnish Resume Deployment

- **Trigger**: Changes to `fi/resume.json` or workflow files
- **Action**: Generates HTML and deploys to GitHub Pages
- **URL**: https://laurisaksi.github.io/resume/

### English Resume Gist Update

- **Trigger**: Changes to `en/resume.json` or workflow files
- **Action**: Updates a GitHub Gist with the latest English resume
- **Purpose**: JSON Resume offers a hosting service that renders resume.json to any theme you would like. The hosting service will automatically detect this when you access `registry.jsonresume.org/your_github_username`
- **URL**: https://registry.jsonresume.org/laurisaksi

## 📚 JSON Resume Standard

This project follows the [JSON Resume](https://jsonresume.org/) standard, which provides:

- Consistent resume structure
- Theme compatibility
- Multiple export formats
- Community-driven development

## 🥩 Raw Formats

[JSON](https://registry.jsonresume.org/laurisaksi.json)

[YAML](https://registry.jsonresume.org/laurisaksi.yaml)

[TEXT](https://registry.jsonresume.org/laurisaksi.txt)

---

_Last updated: August 2025_
