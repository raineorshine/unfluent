# unfluent
[![npm version](https://img.shields.io/npm/v/unfluent.svg)](https://npmjs.org/package/unfluent)

A simple wrapper that calls a Fluent Interface with a configuration object.

> In software engineering, a fluent interface is an object-oriented API whose design relies extensively on method chaining. Its goal is to increase code legibility by creating a domain-specific language (DSL).

<https://en.wikipedia.org/wiki/Fluent_interface>

**Why bad?**

- Javascript has a native object literal syntax (JSON) that is just as DSL-like
- JSON is serializable
- Method chaining obscures mutations

## Install

```sh
npm install --save unfluent
```

## Usage

```js
const commander = require('commander')
const unfluent = require('unfluent')

unfluent(commander, {
  options: [
    ['--d, -d', 'do something']
  ],
})
```
