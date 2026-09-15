<h1 align="center">Mobiwave Email Signature Generator</h1>
<p align="center">An open source html email template builder with drag & drop editor</p>
<img src="./hero.jpg">

## Motivation

We live in an era of increasing vendor lock-in and centralized control. We have seen instances where entire regions are cut off from services due to geopolitical reasons, leaving developers and users stranded. Software should be accessible and reliable, regardless of borders.
 

## Features

- Visual drag-and-drop editor
- Component catalog with ready-to-use blocks: **Menu**, **Header**, **Content**, **Feature**, **Call to Action**, **E-Commerce**, **Footer**
- Spot editing with a component tree (`Block -> Row -> Cell -> Atom`)
- Atom types: `text`, `button`, `divider`, `image`, `menu`
- JSON export/import from the UI
- Import modes: `replace` and `append`
- Template validation + sanitization on import
- Auto-persist to `localStorage` and hydration on reload
- Preview rendered in Shadow DOM to isolate editor styles

## Support

Open source project and completely free to use.

However, the amount of effort needed to maintain and develop new features for the project is not sustainable without proper financial backing. You can support MySigMail Card development via the following methods:

## Development

```sh
pnpm i
pnpm dev
```

## How can I help?

Since the project is undergoing a major rewrite, architectural decisions are still in flux. Direct code contributions might be tricky at this stage, but I welcome feedback and discussions.

**The best way to help right now is to star the repository ⭐** and share it with others. Visibility helps the project grow!

![](./subscribe.gif)

## Commercial Usage

This project is licensed under the **AGPL-3.0**. This means if you include this editor in your own software and make it available to users over a network (SaaS), you must also make your software open source under the same license.

## License

[AGPL-3.0](LICENSE)

Copyright (c) 2026. Mobiwave Innovations.
Adapted from  
