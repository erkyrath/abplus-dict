
This is a spell-check dictionary which (tries to) accept every word in
every Latin-alphabet language. It may be useful for environments where
you can't turn off spell-checking, but you *can* select a custom
dictionary.

(But I've only tested it in English.)

This uses the standard ispell format (`.dic` and `.aff` files),
as described here: https://neovim.io/doc/user/spell.html

To use on MacOS: Copy `acceptall.dic` and `acceptall.aff` into your
`~/Library/Spelling` folder. Then open System Settings and select
the Keyboard pane; hit the Edit button after "Input Sources".
Under "Spelling" select "acceptall (Library)"; *also* select
"Set Up...", check "acceptall (Library)" at the bottom, uncheck
everything else. Hit "Done" (twice) to exit.
