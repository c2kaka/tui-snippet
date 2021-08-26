## TUI-Snippets
vscode snippets extension based on TUI

## Usage Command Line: Quick start

```sh
$ # install node_modules
$ npm i
$ # install vsce
$ npm install -g vsce
$ # build
$ npm run build
$ # package vscode extension
$ npm run release
```

## Snippet tempalte

Markdown file symbol of a specify snippet, like this:

```markdown
---
prefix: button
description: 按钮
scope: typescript,html
---

```html
<button${1: type="${2|text,tel|}"}>
  $0
<button>```
```

- `prefix` defines how this snippet is selected from IntelliSense and tab completion. In this case `button`.
- `description` is the description used in the IntelliSense drop down.
- `scope` Restrict template scope, if not specified, it means no restriction. In this case `typescript` and `html` document.
- markdown body is defines snippet code, muse be hava a code tag.

> How to writing snippet code, pls refre to [vscode-Creating your own snippets](https://code.visualstudio.com/docs/editor/userdefinedsnippets)

