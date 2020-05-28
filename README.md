# Vue Rough Notation

![Rough Notation logo](https://roughnotation.com/images/social.png)

A Vue wrapper for [RoughNotation](https://roughnotation.com/), a small JavaScript library to create and animate annotations on a web page.

[Visit website to see it in action](https://roughnotation.com/)

## Installation

```shell
npm install --save vue-rough-notation
```

## Usage

main.js:

```js
import VueRoughNotation from 'vue-rough-notation';

Vue.use(VueRoughNotation);
```

template:

```html
<RoughNotation
  :show="isShow"
  type="underline"
>
  <span>This is a text</span>
</RoughNotation>
```

## Props

Check [configuring-the-annotation](https://github.com/pshihn/rough-notation#configuring-the-annotation)

**and**

### show

Type: `boolean`

Default: `false`

Whether draws the annotation.

### tag

Type: `string`

Default: `'div'`

String HTML tag name (default: `div`); if falsy (for example `null` or `undefined`), the component will be renderless (the content won't be wrapped in a tag), in this case, only the first child will be rendered
