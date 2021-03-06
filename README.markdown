Configuration files, and setup scripts, for Khan Academy website
developers.  A lot of what's here is Khan Academy-specific:

- Vim filetype plugins conforming to Khan Academy's style guide
- tell ack to skip crap that the deploy script litters
  (eg. combined/compressed CSS/JS files)
- a [pre-commit linter](https://github.com/Khan/khan-linter)

and the rest of it just contains generally useful things, such as

- handy `git` aliases such as `git graph`

This is meant to complement [the dev setup on the Khan Academy Forge](https://sites.google.com/a/khanacademy.org/forge/for-khan-employees/-new-employees-onboard-doc/developer-setup).
The setup scripts here assume you have done the initial setup on that
Forge page (installing npm, etc) before running commands here.

Setup
-----
Clone this repo somewhere (I recommend into a `~/khan/devtools`
directory, but it doesn't really matter), and then run `make` in
the cloned directory:

    mkdir -p ~/khan/devtools
    cd ~/khan/devtools
    git clone https://github.com/Khan/khan-dotfiles.git
    cd khan-dotfiles
    make

This will install your system: installing executables, python
libraries, dotfiles, etc.  It will not overwrite any of your existing
dotfiles but will emit a warning if it sees something it doesn't
understand.

This script is idempotent, so it should be safe to run it multiple times.

You may wish to install
[autojump](https://github.com/joelthelion/autojump) if you're a
frequent user of the terminal to navigate the filesystem.

Hello
-----
Originally extracted from [David's
dotfiles](http://github.com/divad12/dotfiles), with commits and lines
here and there stolen from [Jamie](http://github.com/phleet/dotfiles),
[Desmond](https://github.com/dmnd), and others.  Non-dotfile config
files, and the setup script, written by Craig Silverstein.

Pull requests are welcome!
