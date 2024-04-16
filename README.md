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

## Configuration

Optionally, you can also configure which nodes should be joined if they end up next to each other.
By default, only ordered lists are joined with ordered lists and unordered lists are joined with unordered lists.

```js
import AutoJoiner from 'tiptap-extension-auto-joiner'

new Editor({
  extensions: [
    AutoJoiner.configure({
      elementsToJoin: ["paragraph", "myCustomNode"] //Default ["bulletList", "orderedList"]
    }),
  ],
})
```



