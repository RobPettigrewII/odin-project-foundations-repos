# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This directory holds exercise projects from The Odin Project's Foundations course. It is **not** a single repo. Each subfolder is a separate project, and only some of them are git repos:

| Folder | Git repo | Remote |
|---|---|---|
| `git_test/` | yes | `git@github.com:RobPettigrewII/git_test.git` |
| `odin-recipes/` | yes | `git@github.com:RobPettigrewII/odin-recipes.git` |
| `html-boilerplate/` | no | — |
| `odin-links-and-images/` | no | — |

Run git commands from inside the relevant project folder, not from this parent directory.

## Development

- Every project is plain static HTML. There is no build step, package manager, linter config, or test suite.
- To preview a page, open its `index.html` in a browser.
- `odin-recipes` was formatted with Prettier (see its git history): 2-space indentation, lowercase `<!doctype html>`, self-closing void tags (`<meta ... />`). Keep new files in `odin-recipes` consistent with that style. The other projects aren't formatted with Prettier.

## Structure conventions

- Each project's entry point is `index.html`. Subpages go in a subfolder (`odin-recipes/recipes/`, `odin-links-and-images/pages/`) and use relative links (for example `../index.html`) to get back to the home page.
- Local assets go in `images/`.
- Recipe pages in `odin-recipes/recipes/` all follow the same layout: `<h1>` title, a Home link, an `<img>`, then `<h2>` sections for Description (`<p>`), Ingredients (`<ul>`) and Steps (`<ol>`).

## Context

The user is learning HTML and git through The Odin Project. The exercises are meant to teach those skills, so when asked for help, explain concepts and point the user toward the solution instead of writing the whole lesson for them, unless they ask for a full solution.
