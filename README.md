# ntexup Templates

This repository contains ready-to-use templates for `ntexup` — a text-based, developer-friendly presentation and document generator for academics, researchers, and technical communicators.

`ntexup` is an open-source tool that makes creating professional, math-heavy, and reusable teaching or research materials effortless.

It is built on `Java`, `Nuts`, and `TSON`, combining the simplicity of Markdown with the power of LaTeX and the flexibility of template-driven document generation — all while being version-control friendly.

## Purpose of This Repository
This project serves as a central collection of reusable templates, including:

- Lecture and course templates
- Academic paper and report layouts
- Technical documentation frameworks
- Thematic design presets for slides (themes)
- Custom style and branding examples

All templates here are provided in `.ntx` format, ready to be used directly with `ntexup`.

## Using the Templates

Install `ntexup` from the main repository.

In your `main.ntx` file, just add the following line to include a theme:

```tson
include("github://thevpc/ntexup-templates/classic/v1.0/theme")
```

You can change the themeName (here classic) to one of the available themes:

- classic
- ibtihel

(More themes coming soon)

You can customize the theme by setting some variables in your main.ntx, for example:

```tson
// Set your preferred theme name
themeName = "classic"

// Use an accent color number from 1 to 12
themeColorAccent = 1

// Show palette colors
themeShowPalette = true

// Finally load the theme
include("github://thevpc/ntexup-templates/${themeName}/v1.0/theme")
```

## Creating New Projects from Scratch
You can create a new project from scratch using the ntexup command-line tool.

### Create a Single-File Project
This will create a project with the small template — suitable for quick tests in a single file.

```bash
nuts ntexup --new --template github://thevpc/ntexup-templates/classic/v1.0/templates/small
```

### Create a Multi-File Project
This will create a project with the medium template — a good starting point where slides are split into multiple files.

```bash
nuts ntexup --new --template github://thevpc/ntexup-templates/classic/v1.0/templates/medium
```

### Create a Complex/Large Project
Use this when you are familiar enough with ntexup. It creates a project foundation with many sections and stylings.

```bash
nuts ntexup --new --template github://thevpc/ntexup-templates/classic/v1.0/templates/large
```

Note that you can always edit the .ntx files and choose another template; these are just simple startup projects.


Note also that you can choose templates from themes other than classic.



