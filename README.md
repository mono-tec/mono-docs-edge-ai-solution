# mono-docs-edge-ai-solution

Architecture, design documents and project management for Edge AI solution verification.

## Purpose

This repository manages architecture, design documents and project management artifacts for the Edge AI Solution verification project.

---

## ドキュメント構成

```text
mono-docs-edge-ai-solution
│
├── .github
├── docs
│   ├── concept
│   ├── design
│   ├── project-management
│   ├── architecture
│   └── release
│
├── licenses
│   └── md2pdf-doc-template-LICENSE
│
├── .gitignore
├── package.json
├── package-lock.json
└── README.md
```

---

## Contents

* Concept Design
* Basic Specification
* Project Plan
* Risk Register
* Architecture
* Release Notes

Implementation samples are managed in separate repositories.

---

## PDF Generation

This repository manages design documents in Markdown format.

PDF generation is based on the following template:

https://github.com/tsuna-can-se/md2pdf-doc-template

For the required Node.js packages and build instructions,
please refer to the README of the template project.

The PDF generation environment itself is **not included** in this repository.

---

## Third-party Components

The PDF generation workflow is based on the following project.

* md2pdf-doc-template

The original license is included in:

```text
licenses/md2pdf-doc-template-LICENSE
```

---

## Custom Templates

This project adds the following templates.

* Project Logo
* Concept Design Template
* Basic Specification Template
* Project Plan Template
* Risk Register Template

---

## Related Repositories

| Repository                 | Description            |
| -------------------------- | ---------------------- |
| mono-docs-edge-ai-solution | Design documents       |
| mono-sample-*              | Sample implementations |
| mono-template-*            | Reusable templates     |

---

## PDF Output

Generated PDF files are output to:

```text
docs/output/
```

The required Node.js packages are not included and should be installed locally using npm.
