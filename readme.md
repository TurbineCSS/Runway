Runway
======

A simple, configurable, adaptive framework for [Turbine][1]. Doesn't support IE6 and never will. Runway provides an adaptive layout that matches the users screen width in four steps. Each of the step is configurable in detail so you can easily change the order of your layout columns the match the available space on the screen.


Usage
-----

Configure the layout cell padding in line 4 of `runway-config.cssp` and then either

  - Use `runway.cssp` like any other css framework - include the file and use the classes described below...
  - ...or load `runway-prototypes.cssp` into your style file using the `@load` syntax and extend the protypes (same names as the classes, prefixed with `?`)


Classes and prototypes
----------------------

**Wrapper**: `rw-wrapper` - Clearfixed, provides the layout width

**Rows**: `rw-row` - Clearfixed

**Floats**: `rw-fl` (left), `rw-fr` (right)

**Columns/Cells**: `rw-100`, `rw-90`, `rw-80`, `rw-75`, `rw-70`, `rw-66`,, `rw-65`, `rw-60`, `rw-50`, `rw-40`, `rw-33`, `rw-30`, `rw-25`, `rw-20`, `rw-15`, `rw-10`

**Extra spacing**: `rw-esl` (left), `rw-esr` (right)

**Remove spacing**: `rw-nsl` (left), `rw-nsr` (right)


Presets
-------

The four layouts sizes are by default:

  - 1080px (screen size > 1096px)
  - 960px (screen size between 1096 and 972px)
  - 640px (screen size between 972px and 640px)
  - flexible (mobile devices or screen size > 640px)

These values and the sizes of the layout cells can all be configured in the file `runway-config.cssp`.

  [1]: http://github.com/SirPepe/Turbine
