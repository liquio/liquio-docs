# Liquio Documentation

This repository contains the **static build** of the Liquio documentation site, published at:

- **Production docs**: [https://liquio.github.io/liquio-docs/](https://liquio.github.io/liquio-docs/)
- **Main platform repo**: [https://github.com/liquio/liquio](https://github.com/liquio/liquio)

Liquio is a **low-code GovTech platform using AI to enable rapid digital transformation of public services through intuitive web and mobile applications**, and to support the development of software solutions for the public sector with minimal manual coding. These docs explain the main concepts and how to work with the platform.

## Contents

On the published site, the main sections are:

- **Що таке Liquio?** / **What is Liquio?**
- **Як авторизуватися?** / **How to sign in?**
- **Як створити процес?** / **How to create a process?**
- **Як налаштувати процес?** / **How to configure a process?**
- **Як додати PDF?** / **How to add a PDF?**
- **Як створити реєстр?** / **How to create a register?**
- **Як записати в реєстр?** / **How to write to a register?**
- **Як налаштувати права доступу?** / **How to configure access rights?**
- **Як моніторити процес?** / **How to monitor a process?**

Both **Ukrainian** and **English** versions are available on the site.

## Repository structure

This repo stores the **generated HTML, assets, and images** for the documentation site (built with **MkDocs Material**). It is intended to be used as the GitHub Pages source for `liquio-docs`.

Key top-level items:

- `index.html` – landing page of the docs
- Language and section folders (for example `en/`, `liquio/`, `create-process/`, etc.)
- Static assets under `assets/`, `images/`, and `archive/`

## How this repo is used

- The `main` branch is configured as the **GitHub Pages** source for `https://liquio.github.io/liquio-docs/`.

## Updating the docs

The source for these docs (MkDocs project) lives in a separate repository. The typical update flow is:

1. Update documentation content in the **source docs repo**.
2. Build the static site (MkDocs Material).
3. Publish the generated site output into this repository (overwriting the existing static files).
4. Commit and push to `main` so GitHub Pages redeploys the site.

