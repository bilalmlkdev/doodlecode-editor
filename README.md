<div align="center">

  <a href="https://doodlecode-editor.vercel.app/">
    <img src="https://raw.githubusercontent.com/bilalmlkdev/doodlecode-editor/main/src/assets/favicon.svg" alt="doodlecode-editor logo" height="100">
  </a>

# Doodlecode Editor

Write. Preview. Export. All in real-time.
  A lightweight, zero-setup <br> live code playground for HTML, CSS, and JavaScript.

[![Live Demo](https://img.shields.io/badge/Live_Demo-Visit_Site-black?style=for-the-badge)](https://doodlecode-editor.vercel.app)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](./LICENSE)

</div>

<p align="center">
  <i>Created by <a href="https://bilalmlkdev.vercel.app" target="_blank">Bilal Malik</a></i><br>
  <i>Follow on Github <a href="https://github.com/bilalmlkdev" target="_blank">bilalmlkdev</a></i>
</p>


[![doodlecode-editor Dashboard](https://raw.githubusercontent.com/bilalmlkdev/doodlecode-editor/main/public/preview.png)](https://doodlecode-editor.vercel.app/)


# About Doodlecode Editor

**Doodlecode Editor** is a free, open-source live coding environment for HTML, CSS, and JavaScript. Write code inside three synchronized editors and watch your changes appear instantly in the live preview without saving, refreshing, or configuring anything.

Whether you're prototyping a UI, testing snippets, teaching web development, or building a quick landing page, doodlecode editor provides a clean, distraction-free workspace designed to keep you focused on writing code.

Unlike many online playgrounds that are slow, cluttered, or locked behind subscriptions, doodlecode editor focuses on speed and simplicity.

- **Instant Preview** · Render changes in real time as you type.
- **Clean Interface** · Minimal UI with zero distractions.
- **Auto Save** · Everything is stored automatically in your browser's `localStorage`.
- **Flexible Export** · Export HTML, CSS, JavaScript, ZIP archives, or a standalone HTML file.

Whether you're just starting web development or rapidly testing production ideas, doodlecode editor adapts to your workflow instead of getting in the way.



# Features

- **Live Editors** · HTML, CSS, and JavaScript editors powered by CodeMirror 6 with syntax highlighting, autocomplete, bracket matching, and line numbers.
- **Customization** · Four editor themes, multiple layout modes, adjustable font settings, and responsive workspace layouts.
- **Live Preview** · Instant rendering with automatic background adaptation and fullscreen preview support.
- **Export** · Download individual files, a combined HTML file, or a ZIP archive with optional comment removal and code minification.
- **Smart Saving** · Debounced auto-save with dynamic save status and complete project persistence in `localStorage`.
- **Project Management** · Rename projects at any time with filenames updating automatically during export.
- **Responsive Experience** · Optimized layouts for desktop, tablet, and mobile devices.

# Architecture

Doodlecode editor is built around a clear separation between the editing engine, state management, and the user interface.

Instead of tightly coupling the editors with the preview or export system, the application centralizes code management through custom React hooks and a shared state store. Each editor maintains its own source code while the preview automatically subscribes to changes and updates in real time. This architecture keeps the project predictable, maintainable, and easy to extend.

The entire application runs locally inside the browser without relying on external APIs or server-side processing. All source code, editor preferences, layouts, and project settings are automatically persisted using a debounced `localStorage` save mechanism, allowing projects to survive page refreshes and browser restarts.

Doodlecode editor is a single-page application, with layout switching handled entirely through React state rather than client-side routing.



# License

This project is licensed under the **MIT License**.

```text
MIT License

Copyright (c) 2026 Bilal Malik

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
