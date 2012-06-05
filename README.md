# jade.mode

jade.mode is a jade syntax definition for Coda 2. It is not complete, but it is useful. Please fork, make suggestions or otherwise help as you see fit.

### Installation

Simply check out this repo into either `~/Library/Application Support/Coda 2/Modes` as jade.mode and you're set!

## Features
* Updated for Coda 2
* Highlights all valid HTML5 tags
* Supports embedded HTML
* Highlights all text preceded by `-`, `=` or `!=` as the first non-whitespace character as though it were Javascript
* Highlights save (#{foo}) and unsafe (!{bar}) interpolations
* Highlights doctype declarations (!!! or doctype or <!DOCTYPE style)
* Highlights single-line comments, html comments, and unbuffered
* Highlights jade-specific keywords (block, extends, etc.) when they are the first non-whitespace character.

## Known Issues

* Multi-line comments are unsupported due to limitations of the syntax definition language used by SubEthaEdit & Coda 
  (No capturing groups in regex)
* Code that is not preceded by `-`, `=` or `!=` as the first non-whitespace character is not highlighted
* Code following a tag plus equal sign construct (eg, `p= foo || 'bar'`) is not highlighted
* Embedded JS blocks via script tag are currently not highlighted
* Block expansion (eg, li.foo: a(href='bar')) is not supported only the first tag on the line is highlighted

## Additional Style Scopes

In case you want to tweak your theme a bit, you can add the following scopes in a sort of progressive enhancement. Their absence isn't a big deal.

* *Unbuffered comments* **comment.unbuffered.jade**
* *HTML Generic Tags* **markup.tag.attribute.name.generic.jade**
* *IDs* **markup.tag.attribute.name.id.jade**
* *Classes* **markup.tag.attribute.name.class.jade**
* *Interpolation* **language.variable.interpolation.jade**
* *Escaped Interpolation* **language.variable.interpolation.escaped.jade**

## Author

* Aaron McCall
* Coda 2 Updates+Refactor by [Tom Stoecklein](http://github.com/bluestrike2)

## Credits

James Menera gave me invaluable feedback and encouragement. Thanks, James!