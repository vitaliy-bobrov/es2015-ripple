ES2015 Ripple
==============

[![Bower version](https://badge.fury.io/bo/es2015-ripple.svg)](https://badge.fury.io/bo/es2015-ripple)

A pure javascript (no polymer, no jQuery) lightweight library that adds a Google Material Design ripple effect to elements.

## Bower

  ```bash
  bower install --save es2015-ripple
  ```

## Usage

Include the script in your HTML

  ```html
  <link href="bower_components/es1025-ripple/ripple.css" rel="stylesheet">
  <script src="bower_components/es1025-ripple/ripple.min.js"></script>
  ```

Also you can import SASS styles into your own and compile with your configuration.

```css
@import 'bower_components/es1025-ripple/ripple';
```
### Available SASS configuration variables:
- $ripple-effect-color - Effect color, default `#fff`
- $ripple-effect-time - Effect timing, default `0.45s`
- $ripple-effect-initial-opacity - Effect starting opacity, default `0.4`
- $ripple-effect-scale - Effect max ink scale, default `2.5`

In your own SASS files you can redeclare any of this variables to change defaults. Use `!default` keyword after variable declaration.
Example: `$ripple-effect-time: .5s !default;` - This will change default effect time to 500ms.

Then add `ripple` class to target element

  ```html
  <button class="ripple">Ripple!</button>
  ```

Also you can directly change  effect color with data-attribute `data-ripple-color`, whitch can use any valid CSS color value.

  ```html
  <button class="ripple" data-ripple-color="red">Ripple!</button>

  <button class="ripple" data-ripple-color="#ff00ff">Ripple!</button>
  ```
