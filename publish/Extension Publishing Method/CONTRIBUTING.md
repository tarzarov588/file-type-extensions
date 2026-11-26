# Contributing

![GitHub issues](https://img.shields.io/github/issues/tarzarov588/file-type-extensions?style=for-the-badge)
![GitHub pull requests](https://img.shields.io/github/issues-pr/tarzarov588/file-type-extensions?style=for-the-badge)
![GitHub license](https://img.shields.io/github/license/tarzarov588/file-type-extensions?style=for-the-badge)

Thank you for helping expand **file-type-extensions**.

## Before Opening an Issue

Search open and closed issues to ensure that the extension has not already been submitted or discussed.

## Suggesting a File Extension

Open a GitHub Issue using this information:

**Title:** Add extension: `.ext`

**Include:**

- Extension: `.ext`
- Name of the format
- Category
- Description in Portuguese
- Description in English
- MIME type, if known
- Official specification or documentation
- Extension status:
  - Open
  - Proprietary
  - Legacy
  - Experimental
  - Archive/container
  - Executable
- Associated platforms or software
- Security or forensic warning, if applicable
- Sources used

### Example

```text
Extension: .woff2
Name: Web Open Font Format 2
Category: Fonts
Description PT: Formato de fonte comprimido para uso na web.
Description EN: Compressed font format designed for use on the web.
MIME: font/woff2
Status: Open
Official documentation: https://www.w3.org/TR/WOFF2/
Platforms: Browsers
```

You need to have a **repository** containing the extension you published to our repository.

## Required repository structure

Every new file extension must follow this structure:

```text
<repository-name>/
├── README.md
├── CONTRIBUTING.md
├── CONTRIBUTORS.md
├── LICENSE
├── METADATA.md
└── extensions/
    └── <extension-name>/
        ├── EXPLANATION.md
        └── testing.<extension-name>
```
Example:

```
extensions/
└── woff2/
    ├── EXPLANATION.md
    └── testing.woff2
```

### Required files

- `<extension-name>/`: lowercase folder name without the dot.
- `EXPLANATION.md`: description, category, MIME type, usage, format status, official sources, and information in Portuguese and English.
- `testing.<extension-name>`: harmless example file for testing and identification purposes.
- `README.md`: main project documentation and extension index.
- `CONTRIBUTING.md`: contribution rules.
- `CONTRIBUTORS.md`: contributors list.
- `LICENSE`: MIT license.
- `METADATA.md`: repository and catalog metadata.

## Required structure for executables

Every extension submission must include its own folder under `extensions/`:

```text
<repository-name>/
├── README.md
├── CONTRIBUTING.md
├── CONTRIBUTORS.md
├── LICENSE
├── METADATA.md
├── extensions/
│   └── <extension-name>/
│       ├── EXPLICATION.md
│       └── testing.<extension-name>
└── executable/
    └── bin/
        └── <executable-name>
```
### For non-executable extensions, the `executable/` directory is not required.

For executable extensions, place the executable sample at the repository root under `executable/bin/`. Use a harmless test file. Do not include malware, harmful payloads, private data, or software that performs unauthorized actions. When a runnable sample is not necessary, provide source code or an inert sample instead.

```markdown
## Copyrighted or licensed content

If an extension submission contains copyrighted or licensed material, place it under:

```text
copyright/
└── copyright-extension/
    └── COPYRIGHT.<extension-name>
```

The `<extension-name>` is the extension of the copyrighted file, without the dot.

### Example

```text
copyright/
└── copyright-extension/
    └── COPYRIGHT.md
```

### Required information

Every copyrighted submission must include:

- Proof or clear confirmation of permission to redistribute
- The copyright holder
- The license name and version
- A link to the official license
- The applicable `COPYRIGHT.<extension-name>` file
- A `NOTICE` file, if required by the license
- Any usage restrictions
- `SPDX-License-Identifier` when applicable

Do not submit pirated software, leaked documents, proprietary samples, or private copyrighted content.

The presence of a copyright notice does not grant redistribution rights.

## Commercial fonts

Commercial or proprietary font contributions must be placed under:

```text
commercial/
└── commercial-font-extension/
    └── <commercial-font-name>
```

### Important rules

- Do not submit commercial fonts without the owner's explicit permission.
- Do not upload leaked, cracked, stolen, pirated, or unauthorized font files.
- Do not remove license text, metadata, copyright notices, or usage restrictions.
- Include an official source and redistribution license in `METADATA.md`.
- Personal-use-only fonts cannot be distributed publicly.
- Demonstration or trial files may be submitted only when redistribution is explicitly allowed.
- The presence of a commercial font in this repository does not grant any license to use or redistribute it.

`METADATA.md` must contain the extension information, including:

# Extension metadata

- Extension:
- Format name:
- Category:
- Description PT:
- Description EN:
- MIME type:
- Status:
- Copyright holder:
- License:
- Official source:
- Platforms:
- Commercial font path:
- Redistribution permitted:
- Restrictions:
- Source:
- Extension version:
- Version status:

Example:

```text
commercial/
└── commercial-font-extension/
    └── ExampleFont.otf
```
