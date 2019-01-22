# parcel-plugin-purifycss

A Parcel plugin to remove unused rules from your bundled CSS files in production builds.

## How it works

This plugin uses the [purifycss](https://github.com/purifycss/purifycss) utility to remove unused CSS rules.

PurifyCSS works by reading your source files and checking which CSS selectors are mentioned in your HTML and Javascript code.

This is very useful if you're using a full-featured CSS framework like Bootstrap or Materialize, or even Atomic CSS libraries like Tachyons or BassCSS since you might not use all the provided components and helpers.

## Usage

Just install the plugin as a dependency using yarn or npm and build normally with Parcel. There are no configuration options.

The plugin only applies its changes to production builds. In development mode it is skipped to allow a greater speed of development.

## Installation

```
yarn add parcel-plugin-purifycss
```

or

```
npm install parcel-plugin-purifycss
```

## Issues

This plugin will look for files in your project folder with the following extensions: `html`, `js`, `jsx`, `vue` and `svelte`. Those extensions are hard-coded at the moment, but will change in the future.

## License

```

MIT License

Copyright (c) 2018 Silvio Henrique Ferreira

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
