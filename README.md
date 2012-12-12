# show-keys.el

A global minor mode for emacs that will show what keys you've typed in a window.

## Caveat Hacker

I whipped this together in a giant hurry, but it seems to be stable enough.

## Installation

In your `.emacs`:

```elisp
(add-to-list 'load-path "/path/to/dir-with-show-keys.el/")
(require 'show-keys)
```

## Use

```elisp
M-x show-keys-mode
```

This will create a buffer called `*shown-keys*` which will show the
keys you've typed. Note that it ignores any commands in
`show-keys-ignored-commands`, which by default includes
`self-insert-command`. This keeps the output from being too noisy.

It's not super-sophisticated, but it does catch most things. It's
handy for screencasts or for pairing with someone who doesn't know
emacs that well and is wondering what you're typing. It's also
occasionally handy for figuring out what the heck you just did.

## Screenshot
![screenshot](https://raw.github.com/candera/show-keys.el/master/screenshot.jpg)

## Credits

Thanks to [Stuart Sierra](http://twitter.com/stuartsierra) for an
assist with some of the weird bits.
