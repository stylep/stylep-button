# stylep-button

<img src=giticon.png title=stylep-button align=right height=95>

A simple button style pattern for your next project.

## Install
You can install using the [spm](https://github.com/stylep/stylep) command or install using npm and the project title.

``` shell
spm install button
```

## Usage
``` css
/* button.css */

@import “stylep-button”;

.button {

  /* Button Design Pattern */
  @extend %button-inline;

  /* Customize your button */
  @extend %button-solid;
  --button-color: green;
  --button-text-color: white;
}
```

## Patterns
Placeholder selectors that contain common styles for structure and basic behavior of your buttons.

#### `%button-inline`
This draws a button that displays inline on the page.

##### Variables

```css
--button-cursor: pointer;
--button-display: inline-block;
--button-line-height: 1;
--button-margin: 0 2% 2% 0;
--button-max-width: 100%;
--button-min-width: 44px;
--button-outline: 0;
--button-padding: 13px 18px;
--button-position: relative;
--button-text-align: center;
--button-text-decoration: none;
--button-user-select: none;
--button-vertical-align: middle;
--button-white-space: nowrap;
--button-z-index: 11;
```

#### `%button-block`
This draws a button that expands the width of the containing element.

##### Variables

```css
--button-cursor: pointer;
--button-display: block;
--button-line-height: 1;
--button-margin: 0 2% 2% 0;
--button-max-width: 100%;
--button-min-width: 44px;
--button-outline: 0;
--button-padding: 13px 18px;
--button-position: relative;
--button-text-align: center;
--button-text-decoration: none;
--button-user-select: none;
--button-vertical-align: middle;
--button-white-space: nowrap;
--button-z-index: 11;
--button-width: 100%;
```

#### `%button-group-inline`
This draws containing buttons inline on the page.

#### `%button-group-block`
This draws containing buttons expanded to the width of the containing element.

#### `%button-group-pill`
Combined with another group pattern, you can round off only the first and last button.

## Styles
Customizable presets that give your button a specific style-set.

#### `%button-solid`
Paints your button as a solid object with colors and radius. For added performance the hover state uses the `::after` pseudo-class to render a shadow with only an `opacity` transition.

##### Variables

```css
--button-color: #333;
--button-hover-color: #555;
--button-text-color: #fff;
--button-radius: 4px;
--button-shadow: none;
--button-transition: background-color .3s ease-in-out;
--button-will-change: background-color;

/* State Opacity  */
--button-hover-opacity: 1;
--button-disabled-opacity: .35;
```

#### %button-hollow
Same as it’s solid counterpart, but it is drawn with a border instead.

##### Variables

```css
--button-color: transparent;
--button-hover-color: #555;
--button-text-color: #555;
--button-hover-text-color: #fff;
--button-radius: 4px;
--button-shadow: none;
--button-border: 1px solid #555;
--button-transition: background .3s ease-in-out, color .3s ease-in-out;

/* State Opacity  */
--button-hover-opacity: 1;
--button-disabled-opacity: .35;
```

#### %button-circle-solid
Paints your button as a solid object with colors, shadow and rounded radius.

##### Variables

```css
--button-radius: 50%;
--button-padding: 15px;
```

#### %button-circle-hollow
Paints your button as a outlined object with color, shadow and rounded radius.

##### Variables

```css
--button-radius: 50%;
--button-padding: 15px;
```

## License
This project is licensed under the MIT [license](LICENSE).

