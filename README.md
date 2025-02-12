# dragonruby-completions for VSCode
A set of Itellisense auto-completions (code snippets) for DragonRuby

Add the `.vscode` folder to your project directory.

You'll also need to enable code completion. Go to the VSCode Settings, search for `editor.tabCompletion` in the settings search bar.
Then under the setting, you can selected to turn it on.
 * on
 * off (default)
 * onlySnippets

> Personally, I only turned it on for Code Snippets, and did it in the "user" profile section, so that it wouldn't follow me around project-to-project.

## What does this do?

The file `ruby.code-completions` provides a small set of auto-completions for creating different hash primitives and other convienence completions.

## Creating simple hashes

to create a simple sprite hash, use the following:
 `.make_sprite`

 which will create a hash with all the basic key/value pairs for a sprite, you can tab to each of the values for quick creation.

 `{x: x_position, y: y_position, w: width, h: height, path: "path_to_sprite", primitive_marker: :sprite}`

 there are also the following `.make_` auto-completions available:

 * `.make_label`
 * `.make_solid`
 * `.make_border`
 * `.make_line`

## Adding just a primitive marker

another set of auto-completions available are completions to just add the primitive marker such as:
 `.to_sprite`
 which will add the following key/value pair upon copletion:

 `, primitive_marker: :sprite`

 the other `.to_*` completions availble are:

 * `.to_label`
 * `.to_solid`
 * `.to_border`
 * `.to_line`

## Color keys and hashes

You can also added a color hash using the following:

* `.make_color`
  Which adds the following to your code: `{r: $red, g: $green, b: $blue}`
* `.make_color_keys`
  Which adds the following to your code: `r: $red, g: $green, b: $blue`, it's convenient for adding to an existing hash, usually an output primitive.

## Other Hashes

You can also added a point or rect hash using the following:

* `.make_rect_hash`
  Which adds the following to your code: `{x: $x, y: $y, w: $width, h: $height}`
* `.make_point_hash`
  Which adds the following to your code: `{x: $x, y: $y}`
