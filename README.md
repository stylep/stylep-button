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
  @mixin button-inline;

  /* Customize your button */
  @mixin button-solid green, #000, #fff;
}
```

## Patterns
Placeholder selectors that contain common styles for structure and basic behavior of your buttons.

#### `button-inline`
This draws a button that displays inline on the page.

##### Options

* `$button-padding: 15px` Space inside the button
* `$button-margin: 0 2% 2% 0` Space around the button

#### `button-block`
This draws a button that expands the width of the containing element.

##### Options

* `$button-padding: 15px` Space inside the button
* `$button-margin: 0 2% 2% 0` Space around the button

#### `button-group-inline`
This draws containing buttons inline on the page.

##### Options

* `$button-group-padding: 0` Space inside the group
* `$button-group-margin: 0 0 2%` Space around the group

#### `button-group-block`
This draws containing buttons expanded to the width of the containing element.

##### Options

* `$button-group-padding: 0` Space inside the group
* `$button-group-margin: 0 0 2%` Space around the group

## Styles
Customizable presets that give your button a specific style-set.

#### `button-solid`
Paints your button as a solid object with colors and radius. For added performance the hover state uses the `::after` pseudo-class to render a shadow with only an `opacity` transition.

##### Options

* `$button-color: #333`
* `$button-hover-color: #555`
* `$button-text-color: #fff`
* `$button-hover-shadow: none`
* `$button-radius: 4px`
* `$button-duration: .3s`
* `$button-disabled-opacity: .35`

#### button-hollow
Same as it’s solid counterpart, but it is drawn with a border instead.

##### Options

* `$button-color: #555`
* `$button-hover-text-color: #fff`
* `$button-hover-shadow: none`
* `$button-radius: 4px`
* `$button-duration: .3s`
* `$button-disabled-opacity: .35`

#### `button-group-pill`
Combined with another group pattern, you can round off only the first and last button.

## License
This project is licensed under the MIT [license](LICENSE).

