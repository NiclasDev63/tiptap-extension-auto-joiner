# Tiptap Extension: AutoJoiner

## Install

NPM
```
$ npm install tiptap-extension-auto-joiner
```

Yarn
```
$ yarn add tiptap-extension-auto-joiner
```

## Usage

```js
import AutoJoiner from 'tiptap-extension-auto-joiner'

new Editor({
  extensions: [
    AutoJoiner,
  ],
})
```
This extension provides the expected behavior for lists, e.g. joining two adjacent lists to one.
It can be extended to join not only lists, but all types of nodes that are next to each other, such as paragraphs or custom nodes.
