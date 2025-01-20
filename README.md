# dragonruby-completions
A set of Itellisense auto-completions (code snippets) for DragonRuby

Add the `.vscode` folder to your project directory.

The file `ruby.code-completions` provides a small set of auto-completions for creating different hash primitives.

## Creating simple hashes

to create a simple sprite hash, use the following:
 `.make_sprite`

 which will create a hash with all the basic key/value pairs for a sprite, you can tab to each of the values for quick creation.

 `{x: x_position, y: y_position, w: width, h: hieght, path: "path_to_sprite", primitive_marker: :sprite}`

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
