# stylep-button
A simple button style pattern for your next project.

## Install
``` shell
# NPM
npm i --save-dev stylep-button

# Bower
bower install stylep-button
```

## Usage
``` css
/* button.css */

@import “stylep-button”;

.button {

  /* Button Design Pattern */
  @extend %button-inline;

  /* Customize your button */
  @mixin button-solid navy, blue, #fff, 0 1px 1px #000;

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

#### `@extend %button-block`
This draws a button that expands the width of the containing element.

## Styles
Customizable presets that give your button a specific style-set.

### button-solid
Paints your button as a solid object with colors, shadow and radius.
```css
/* navy background that shifts to blue on hover, in white text, rounded by 3px with a black box shadow that expands spread on hover  */
@mixin button-solid navy, blue, #fff, 3px, 0 0 0 black, 0 0 5px black;
```

### button-hollow
Paints your button as a outlined object with color, shadow and radius.
```css
/* navy text and border that shifts to blue on hover, with a transparent background, rounded by 3px and no shadow */
@mixin button-hollow navy, blue, transparent, 3px, 1px, none, none;
```

