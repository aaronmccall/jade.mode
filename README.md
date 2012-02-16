# jade.mode


jade.mode is a jade syntax definition for SubEthaEdit & Coda. 

## Usage

### Installation

Simply check out this repo into either `~/Library/Application Support/Coda/Modes` or `~/Library/Application Support/SubEthaEdit/Modes`, be sure to name the directory `jade.mode`.

## Known Issues

* Multi-line comments are unsupported
* Code that is not preceded by `-`, `=` or `!=` is not highlighted
* Code following a tag plus equal sign construct (eg, `p= foo || 'bar'`) is not highlighted
* Embedded JS blocks via script tag are currently not highlighted

## Author

Aaron McCall

### Credits

James Menera gave me invaluable feedback and encouragement. Thanks, James!

