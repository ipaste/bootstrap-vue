# Color Variants and CSS class mapping

> Below are the variants available when using the default Bootstrap V4 CSS.
When using Boostrap-Vue components, the variants are refered to
by their varaint name, rather than by the underlying CSS classname

## Base variants
* `primary` - <span class="text-primary">Primary</span>
* `secondary` - <span class="text-secondary">Secondary</span>
* `success` - <span class="text-success">Success</span>
* `warning` - <span class="text-warning">Warning</span>
* `danger` - <span class="text-danger">danger</span>
* `info` - <span class="text-info">Info</span>
* `light` - <span class="text-light">Light</span>
* `dark` - <span class="text-dark">Dark</span>

The base variants will translate to various Bootstrap V4 contextual class
names based on the compoennt (and variant purpose) where they are used.

## Background and border variants
All the **base variants** plus:
* `transparent`

These translate to class names `bg-<variant>` for backgrounds and
`border-<variant>` for borders.

These variants are used by components (such as `<b-card>`, `<b-jumbotron>`
and `<b-modal>`) that provide `bg-variant`, `*-bg-variant`, `border-variant`
and `*-border-variant` props

## Text variants
All the **base variants** plus:
* `muted`
* `white`
* `black`

These translate to class names `text-<variant>`

These variants are used by components (such as `<b-card>`, `<b-jumbotron>`
and `<b-modal>`) that provide `text-variant` and `*-text-variant` props


## Component specific variants
Some Bootstrap V4 components requiire aditional CSS styling, or aditional
pseudo selector styling (i.e buttons), and hence have their own underlying
variant CSS classes.


### Alert variants
All the **base variants**

These translate to class names `alert-<variant>`.


### Badge variants
All the **base variants**

These translate to class names `badge-<variant>`.


### Button variants
All the **base variants** plus:
* `outline-<base variant>`
* `link` which renders the button with the look of a link but retains button padding and margins.

These translate to class names `btn-<variant>` and `btn-outline-<variant>`.


### Table variants
All the **base variants**:

These translate to class names `table-<variant>`.
When the table is in `inverse` mode, the variants translate to
the `bg-<variant>` classes.


## Using variant classes

You may also use the underlying class names directly on elements (and some
components) via the standard HTML `class="..."` attribute.

## Creating custom variants
When creating custom variants, follow the Bootstrap V4 varian CSS class naming
scheme and they will become available to the various components that use that
scheme (i.e. create a custom CSS class `btn-purple` and `purple` becomes a
vailid variant to use on `<b-button>`).
