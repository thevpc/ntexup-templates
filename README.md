# ntexup Templates

This repository contains ready-to-use templates for `ntexup` — a text-based, developer-friendly presentation and document generator for academics, researchers, and technical communicators.

`ntexup` is an open-source tool that makes creating professional, math-heavy, and reusable teaching or research materials effortless.

It is built on `Java`, `Nuts`, and `TSON`, combining the simplicity of Markdown with the power of LaTeX and the flexibility of template-driven document generation — all while being version-control friendly.

## Purpose of This Repository
This project serves as a central collection of reusable templates, including:

- Lecture and course templates
- Academic paper and report layouts
- Technical documentation frameworks
- Thematic design presets for slides
- Custom style and branding examples

All templates here are provided in .ntx format, ready to be used directly with `ntexup`.

## Using the Templates
Install ntexup from the main repository.
the in your main.ntx file just drop the following


```java
include("github://thevpc/ntexup-templates/classic/v1.0/theme")
```

you can change the themeName (here `default`) with one of the available followings :

- default
- ibtihel

___(More themes coming soon)___




## creating new projects from scratch
in this repo

### create a single file project

this will create a project with the template `default` that you can edit in a single file. use this for testing.

```bash
nuts ntexup --new --template github://thevpc/ntexup-templates/main/default/v1.0/boot/small
```

### create a multi-file project

this will create a project with the template `default` that you can edit in a single file. 
If you are not sure what to choose, choose this. this is good start. it ll help you create
slides each in a file apart.

```bash
nuts ntexup --new --template github://thevpc/ntexup-templates/main/default/v1.0/boot/default
```

### create a complex/large project
this will create the foundation of a big project with many sections and stylings.
If you ca use this when you are familiar enough with ntexup.

```bash
nuts ntexup --new --template github://thevpc/ntexup-templates/main/default/v1.0/boot/large
```

note that you can always change the ntx file content and choose another template, this is a simple startup project only

note also that you can change another templates (other than 'default')


