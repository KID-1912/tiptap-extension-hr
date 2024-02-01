# tiptap-extension-hr

<h3 align="center">
    Extension to add dividers(horizontal) to your tiptap content.
</h3>

<br/>

<p align="center">
  <a href="https://www.npmjs.com/package/tiptap-extension-hr">
    <img
     alt="NPM URL"
     src="https://img.shields.io/badge/npm-tiptapExtensionHr?logo=npm">
  </a>
  <img
     alt="version"
     src="https://img.shields.io/badge/version-1.0.0-blue">
</p>

<br>

---

## Install

```shell
npm install tiptap-extension-hr -S
```

## Usage

```js
import Hr from "tiptap-extension-hr";

const editor = new Editor({
  element: document.querySelector(".editor"),
  extensions: [StarterKit, Hr],
});

editor
  .chain()
  .focus()
  .insertContent([{ type: "hr" }])
  .run();
```

## Options

Customize the line style with the optional style option.

```js
  extensions: [
    StarterKit,
    Image.configure({ inline: true }),
    Hr.configure({
      style: 'border-style: solid;border-width: 1px 0 0;border-color: rgba(0,0,0,0.1);transform-origin: 0 0;transform: scale(1, 0.5);'
    }),
  ],
```

## Relations

**tiptap:** https://tiptap.dev/

**tiptap-appmsg-editor:** https://github.com/KID-1912/tiptap-appmsg-editor
