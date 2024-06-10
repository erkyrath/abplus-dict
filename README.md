# abplus-dict: a spellcheck dictionary that never complains

- Created by Andrew Plotkin <erkyrath@eblong.com>
- [More info on this project](https://blog.zarfhome.com/2024/06/neutering-spellcheck-on-macos)

This is a spell-check dictionary which (tries to) accept every word in
every Latin-alphabet language. It may be useful for environments where
you can't turn off spell-checking, but you *can* select a custom
dictionary.

(But I've only tested it in English.)

This uses the standard ispell format (`.dic` and `.aff` files),
as described [here][vimdoc] amd [here][hundoc].

[vimdoc]: https://neovim.io/doc/user/spell.html#spell-wordlist-format
[hundoc]: https://linux.die.net/man/4/hunspell

To use on MacOS:

- Copy `abplus-dict.dic` and `abplus-dict.aff` into your `~/Library/Spelling` folder.
- Open System Settings.
- Select "Keyboard".
- Press the "Edit..." button next to "Input Sources".
- Open the dropdown menu for "Spelling". (It's set to "Automatic by Language" by default.)
- Scroll all the way down to the bottom of the menu and select "Set Up..."
- In the dialogue box, check "abplus-dict (Library)" and uncheck every other checkbox. (It refuses to uncheck *every* box; you have to leave at least one checked.)
- Hit "Done".
- Open the dropdown menu for "Spelling" again. Scroll down and select "abplus-dict (Library)". Not the "Set Up..." entry, but the one above it.
- Hit "Done".
- Quit System Settings.
- Quit and restart any apps you have open to pick up the new spellcheck setting.

