Steps to Automate Brew Installation from a Mac to another Mac
---

On the first Mac: Export your list of installed apps
Use the brew bundle command to create a Brewfile in your home directory with all installed formulae, casks, and taps.

**brew bundle dump --describe --file=~/Brewfile**

Copy the Brewfile to the second Mac


Put the Brewfile in your home directory:

**brew bundle --file=~/Brewfile**

It will install:

* All your previously installed CLI tools (brew install)
* GUI apps (brew install --cask)
* Taps (custom sources)
