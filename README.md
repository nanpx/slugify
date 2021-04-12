# slugify

![NPM Build](https://github.com/nanpx/slugify/actions/workflows/npm-build.yml/badge.svg) [![current version](https://img.shields.io/npm/v/@nanpx/slugify.svg?style=flat-square)](https://www.npmjs.com/package/@nanpx/slugify)

## Install

```bash
npm install @nanpx/slugify
```

## Use

```javascript
(() => {
  'use strict';

  const Slugify = require('@nanpx/slugify');
  const title = 'Page Title';
  const slug = Slugify.parseSync(title);

  console.log(slug); // 'page-title'

  // or promise version
  Slugify.parse(title)
  .then((slug) => console.log(slug)); // 'page-title'
})();
```
