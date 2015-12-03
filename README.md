# stylep-button

<img src=giticon.png title=stylep-button align=right height=95>

A simple button style pattern for your next project.

## Install
``` shell
npm i --save-dev stylep-button
```

## Usage
``` css
/* button.css */

@import “stylep-button”;

.button {

  /* Button Design Pattern */
  @extend %button-inline;

  /* Customize your button */
  @mixin button-solid navy, blue;

  /* or roll your own */
  background-color: blue;
  box-shadow: 0 1px 1px #000;
  color: #fff;
}
```

## Patterns
Placeholder selectors that contain common styles for structure and basic behavior of your buttons.

#### `@extend %button-inline;`
This draws a button that displays inline on the page.

#### `@extend %button-block;`
This draws a button that expands the width of the containing element.

## Styles
Customizable presets that give your button a specific style-set.

### button-solid
Paints your button as a solid object with colors, shadow and radius.

##### Options

* `$color-passive: #999` Background color by default
* `$color-hover: #666` Backgound color on hover or focus
* `$color-text: #fff` Color of the inner text by default
* `$radius-size: 4px` Size of the border radius by default
* `$shadow: 0 0 6px rgba(50, 50, 50, .5)` Box shadow style on hover and focus

##### Example
```css
/* navy background that shifts to blue on hover, in white text, rounded by 3px with a black box shadow that expands spread on hover  */
@mixin button-solid navy, blue, #fff, 3px, 0 0 5px black;
```

### button-hollow
Paints your button as a outlined object with color, shadow and radius.

##### Options

* `$color-passive: #999` Border and text color by default
* `$color-hover: #666` Border and text color on hover or focus
* `$color-background: transparent` Optional background-color, made transparent by default
* `$radius-size: 4px` Size of the border radius by default
* `$border-width: 1px` Width of the border by default
* `$shadow: none` Box shadow style on hover and focus

##### Example
```css
/* navy text and border that shifts to blue on hover, with a transparent background, rounded by 3px and no shadow */
@mixin button-hollow navy, blue, transparent, 3px, 1px, none;
```

