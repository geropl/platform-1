## Structure

> **workflow** - is a common term for user story / business workflow

- **utils** - basic reusable constants, functions and services without knowledge of a workflow
- **blocks** - basic reusable view components (ui-kit) without knowledge of a workflow
- **widgets** - main futures serves a workflow by combining utils or / and blocks
- **pages** - widgets bindings (entry points and main layouts) to web view

**Utils**, **blocks** and **widgets** follows a file-structure pattern:

- **index.ext** - reexports
- **entityN.ext** - main entity code
- ?**entityN** - optional folder with additional components
  - **index.ext** - reexports
  - **entityNM.ext** - main subentity code
  - ?**entityNM** - another folder... and so on like a **fractal**

**Pages** follows [next.js guide](https://nextjs.org/docs/basic-features/pages)
