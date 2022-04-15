# Astro Head

Batteries-included Astro component for your `<head>`.

## Features

* Global tags (utf-8, viewport)
* Primary metadata (title, description)
* Favicon paths
* SEO tags
* Analytics
* Minimal configuration

## Installation

```bash
npm i astro-head
```

## Usage

Inside your Astro pages, add this to your `<head>`:

```astro
---
import Head from 'astro-head';

const title = 'Page Title';
const description = 'Short description of the page.';
const analytics = {
  provider: 'google',
  id: 'XXXXXX',
};
---
<html lang="en">
  <head>
    <Head {title} {description} {analytics} />
  </head>
  <body>
    <!-- page content -->
  </body>
</html>
```
