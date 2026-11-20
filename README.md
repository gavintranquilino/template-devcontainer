# template-CI

A foundation for new repositories that adds lightweight pull request checks to [template-base](https://github.com/gavintranquilino/template-base). It provides coding, documentation, and contribution conventions, plus checks that keep documentation consistent. Projects can extend it for their languages and tools.

## Start Here

* **Adopting or extending the template:** Follow [Template Usage](docs/guides/template-usage.md).
* **Contributing:** Read [Contributing](CONTRIBUTING.md) for the branch, review, and verification workflow.
* **Writing code:** Follow [Coding Style](docs/coding-style.md).
* **Writing documentation:** Follow [Documentation](docs/documentation.md). The [Documentation Map](docs/README.md) lists the included documents.
* **AI assistants:** Read [AGENTS.md](AGENTS.md) for repository instructions.

## Included Files

```text
.
├── README.md                     Repository introduction
├── CONTRIBUTING.md               Contribution and review workflow
├── AGENTS.md                     Instructions for AI assistants
├── .gitignore                    Local files to exclude from version control
├── .gitattributes                Line-ending normalization
├── .editorconfig                 Shared editor settings
├── .github/
│   ├── pull_request_template.md  Pull request description template
│   └── workflows/
│       └── checks.yml            Checks that run on pull requests
├── tools/
│   ├── README.md                 Tool descriptions and local usage
│   └── scripts/                  Check scripts and their configuration
└── docs/
    ├── README.md                 Documentation map
    ├── coding-style.md           Shared style and an area for language rules
    ├── documentation.md          Documentation placement and conventions
    ├── glossary.md               Shared terms and acronyms
    └── guides/
        ├── README.md             Guide index
        └── template-usage.md     Adoption and extension checklist
```

## Repository Structure

Choose a source layout that fits the project. A single-project repository can keep its source and tests at the root. A monorepo can organize applications, packages, or services in separate directories, each with its own setup and verification instructions.

Root conventions apply throughout the repository. Local guidance can extend them for a component and must explicitly identify any exceptions. Explain component boundaries and shared workflows in the root README as the repository grows.

## Included Checks

Pull requests run the checks described in [Tools](tools/README.md). They need only Python 3 and Git, and you can run them locally with the same commands.

## Extending the Base

This template builds on template-base and adds lightweight pull request checks. The checks run in GitHub Actions and need only Python 3 and Git. It requires no package manager or build system. Add language rules, development environments, command-line tools, and automated checks in derived templates or individual repositories. Each addition must include the files and instructions needed to use it.

When adopting the template, replace this introduction with the project's purpose, layout, and setup instructions. Keep the shared conventions and adapt them where needed, as [Template Usage](docs/guides/template-usage.md) describes.
