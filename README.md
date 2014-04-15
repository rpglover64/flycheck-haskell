flycheck-haskell — Flycheck for Haskell
=======================================

Configure [Flycheck][] for Haskell:

- Add source directories from your cabal project to the search path
- Add build files and auto-generated files from Cabal to the search path
- Use package databases from the current Cabal sandbox

Installation
------------

As usual, from [MELPA][] and [Marmalade][].

In your [`Cask`][cask] file:

```cl
(source gnu)
(source melpa)

(depends-on "flycheck-haskell")
```

In your `init.el`:

```cl
(eval-after-load 'flycheck
  '(add-hook 'flycheck-mode-hook #'flycheck-haskell-setup))
```

Usage
-----

Just use Flycheck as usual in your Cabal projects.

Customization
-------------

- <kbd>M-x customize-group RET flycheck-haskell</kbd>

License
-------

This program is free software: you can redistribute it and/or modify it under
the terms of the GNU General Public License as published by the Free Software
Foundation, either version 3 of the License, or (at your option) any later
version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with
this program.  If not, see http://www.gnu.org/licenses/.

See [`COPYING`][copying] for details.

[Flycheck]: https://github.com/flycheck/flycheck
[Cask]: https://github.com/cask/cask
[MELPA]: http://melpa.milkbox.net
[Marmalade]: http://marmalade-repo.org/
[COPYING]: https://github.com/flycheck/flycheck-haskell/blob/master/COPYING