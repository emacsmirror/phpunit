# phpunit.el

[![License GPL 3][badge-license]][LICENSE]
[![travis][badge-travis]][travis]

Manage the [PHPUnit][] tests from Emacs.

## Installation

The recommended way to install ``phpunit.el`` is via [MELPA][]:

    M-x package-install phpunit.el

or [Cask][]:

	(depends-on "phpunit.el")


## Usage

### Available commands

These functions are available :
* `phpunit-current-test`: launch unit tests for the current test in a class
* `phpunit-current-class`: launch unit tests for the current class
* `phpunit-current-project`: launch all unit tests

You can create some key bindings with these commands:

```lisp
(define-key web-mode-map (kbd "C-x t") 'phpunit-current-test)
(define-key web-mode-map (kbd "C-x c") 'phpunit-current-class)
(define-key web-mode-map (kbd "C-x p") 'phpunit-current-project)
```

## Development

### Cask

``phpunit.el`` use [Cask](https://github.com/cask/cask) for dependencies
management. Install it and retrieve dependencies :

    $ curl -fsSkL https://raw.github.com/cask/cask/master/go | python
    $ export PATH="$HOME/.cask/bin:$PATH"
    $ cask


### Tests

Launch unit tests :

    $ make clean test


## Support / Contribute

See [here](CONTRIBUTING.md)



## Changelog

A changelog is available [here](ChangeLog.md).


## License

See [LICENSE](LICENSE).


## Contact

Nicolas Lamirault <nicolas.lamirault@gmail.com>


[badge-license]: https://img.shields.io/badge/license-GPL_2-green.svg?style=flat
[LICENSE]: https://github.com/nlamirault/phpunit.el/blob/master/LICENSE
[travis]: https://travis-ci.org/nlamirault/phpunit.el
[badge-travis]: http://img.shields.io/travis/nlamirault/phpunit.el.svg?style=flat
[GNU Emacs]: https://www.gnu.org/software/emacs/
[MELPA]: http://melpa.milkbox.net/
[Cask]: http://cask.github.io/
[Issue tracker]: https://github.com/nlamirault/phpunit.el/issues
[PHPUnit]: http://phpunit.de
