[![Published on NPM](https://img.shields.io/npm/v/@advanced-rest-client/authorization-data-saver.svg)](https://www.npmjs.com/package/@advanced-rest-client/authorization-data-saver)

[![Build Status](https://travis-ci.org/advanced-rest-client/authorization-data-saver.svg?branch=stage)](https://travis-ci.org/advanced-rest-client/authorization-data-saver)

[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/advanced-rest-client/authorization-data-saver)


# &lt;authorization-data-saver&gt;

An element responsible for applying authorization data to the request and requesting auth data from the user.

It dispatches `resend-auth-request` custom event after the user accept dialog with data. The handler should send the request again with updated data.

## Example:

## API components

This components is a part of [API components ecosystem](https://elements.advancedrestclient.com/)

## Usage

### Installation
```
npm install --save @advanced-rest-client/authorization-data-saver
```

### In an html file

```html
<html>
  <head>
    <script type="module">
      import './node_modules/@advanced-rest-client/authorization-data-saver/authorization-data-saver.js';
    </script>
  </head>
  <body>
    <authorization-data-saver></authorization-data-saver>
  </body>
</html>
```

### In a Polymer 3 element

```js
import {PolymerElement, html} from './node_modules/@polymer/polymer/polymer-element.js';
import './node_modules/@advanced-rest-client/authorization-data-saver/authorization-data-saver.js';

class SampleElement extends PolymerElement {
  static get template() {
    return html`
    <authorization-data-saver></authorization-data-saver>
    `;
  }
}
customElements.define('sample-element', SampleElement);
```

### Installation

```sh
git clone https://github.com/advanced-rest-client/authorization-data-saver
cd api-url-editor
npm install
npm install -g polymer-cli
```

### Running the demo locally

```sh
polymer serve --npm
open http://127.0.0.1:<port>/demo/
```

### Running the tests
```sh
polymer test --npm
```
