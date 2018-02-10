# slugify

[![travis.ci](https://img.shields.io/travis/nanpx/slugify.svg?style=flat-square)](https://travis-ci.org/nanpx/slugify) [![current version](https://img.shields.io/npm/v/@nanpx/slugify.svg?style=flat-square)](https://www.npmjs.com/package/@nanpx/slugify)

<!-- MarkdownTOC autolink="true" bracket="round" depth="2" indent="    " -->

- [Install](#install)
- [Use](#use)

<!-- /MarkdownTOC -->

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
