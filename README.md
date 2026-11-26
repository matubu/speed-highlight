<h3 align="center">
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/logos/exports/1544x1544_circle.png" width="100" alt="Logo"/><br/>
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
	Catppuccin for <a href="https://github.com/speed-highlight/core">Speed Highlight</a>
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
</h3>

<p align="center">
	<a href="https://github.com/matubu/speed-highlight/stargazers"><img src="https://img.shields.io/github/stars/matubu/speed-highlight?colorA=363a4f&colorB=b7bdf8&style=for-the-badge"></a>
	<a href="https://github.com/matubu/speed-highlight/issues"><img src="https://img.shields.io/github/issues/matubu/speed-highlight?colorA=363a4f&colorB=f5a97f&style=for-the-badge"></a>
	<a href="https://github.com/matubu/speed-highlight/contributors"><img src="https://img.shields.io/github/contributors/matubu/speed-highlight?colorA=363a4f&colorB=a6da95&style=for-the-badge"></a>
</p>

<p align="center">
	<img src="assets/preview.webp"/>
</p>

## Previews

<details>
<summary>🌻 Latte</summary>
<img src="assets/latte.webp"/>
</details>
<details>
<summary>🪴 Frappé</summary>
<img src="assets/frappe.webp"/>
</details>
<details>
<summary>🌺 Macchiato</summary>
<img src="assets/macchiato.webp"/>
</details>
<details>
<summary>🌿 Mocha</summary>
<img src="assets/mocha.webp"/>
</details>

## Usage

Catppuccin is now [included in Speed Highlight](https://github.com/speed-highlight/core/tree/main/src/themes): the four flavors ship in the `@speed-highlight/core` package as `catppuccin-latte.css`, `catppuccin-frappe.css`, `catppuccin-macchiato.css` and `catppuccin-mocha.css`.

1. Install the package.

   ```sh
   npm i @speed-highlight/core
   ```

2. Import the stylesheet of your preferred flavor.

   ```js
   import '@speed-highlight/core/themes/catppuccin-mocha.css'; // or latte, frappe, macchiato
   ```

3. Mark your code blocks with a `shj-lang-*` class and call `highlightAll()`.

   ```html
   <div class="shj-lang-js">console.log('hello')</div>

   <script type="module">
   	import { highlightAll } from '@speed-highlight/core';
   	highlightAll();
   </script>
   ```

To render a string instead of a page element (React, Vue, Svelte, ...), use `highlightHTML(code, lang)` and put its output inside an element with the `shj-lang-<lang>` class, as shown in the [Speed Highlight README](https://github.com/speed-highlight/core#readme).

## 🙋 FAQ

- Q: **_"How can I follow the system light/dark setting?"_**\
  A: Load two flavors and let the browser pick one with a media query:

  ```html
  <link rel="stylesheet" media="(prefers-color-scheme: light)" href="node_modules/@speed-highlight/core/dist/themes/catppuccin-latte.css">
  <link rel="stylesheet" media="(prefers-color-scheme: dark)" href="node_modules/@speed-highlight/core/dist/themes/catppuccin-mocha.css">
  ```

## 💝 Thanks to

- [Mathias](https://github.com/matubu)

&nbsp;

<p align="center">
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/footers/gray0_ctp_on_line.svg?sanitize=true" />
</p>

<p align="center">
	Copyright &copy; 2021-present <a href="https://github.com/catppuccin" target="_blank">Catppuccin Org</a>
</p>

<p align="center">
	<a href="https://github.com/catppuccin/catppuccin/blob/main/LICENSE"><img src="https://img.shields.io/static/v1.svg?style=for-the-badge&label=License&message=MIT&logoColor=d9e0ee&colorA=363a4f&colorB=b7bdf8"/></a>
</p>
