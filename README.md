# jade.mode

jade.mode is a jade syntax definition for SubEthaEdit & Coda. It is not complete, but it is useful. Please fork, make suggestions or otherwise help as you see fit.

## Coda 2 support!

@bluestrike2 (Tom Stoecklein) has created a Coda 2 version of the mode. It is available in the [coda2_master branch](https://github.com/aaronmccall/jade.mode/tree/coda2_master)

### Installation

Simply check out this repo into either `~/Library/Application Support/Coda/Modes` or `~/Library/Application Support/SubEthaEdit/Modes`, be sure to name the directory `jade.mode`.

## Features
* Highlights all valid HTML5 tags
* Supports embedded HTML
* Highlights all text preceded by `-`, `=` or `!=` as the first non-whitespace character as though it were Javascript
* Highlights save (#{foo}) and unsafe (!{bar}) interpolations
* Highlights doctype declarations (!!! or doctype or <!DOCTYPE style)
* Highlights single-line comments
* Highlights jade-specific keywords (block, extends, etc.) when they are the first non-whitespace character.

## Known Issues

* Multi-line comments are unsupported due to limitations of the syntax definition language used by SubEthaEdit & Coda 
  (No capturing groups in regex)
* Code that is not preceded by `-`, `=` or `!=` as the first non-whitespace character is not highlighted
* Code following a tag plus equal sign construct (eg, `p= foo || 'bar'`) is not highlighted
* Embedded JS blocks via script tag are currently not highlighted
* Block expansion (eg, li.foo: a(href='bar')) is not supported only the first tag on the line is highlighted

## Authors

Aaron McCall
Tom Stoecklein (Coda 2 refactor)

## Credits

James Menera gave me invaluable feedback and encouragement. Thanks, James!