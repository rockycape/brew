My brewfile
---
Steps to Automate Brew Installation from a Mac to another Mac
1. On the first Mac: Export your list of installed apps
Use the brew bundle command:

**brew bundle dump --describe --file=~/Brewfile** (This creates a Brewfile in your home directory with all installed formulae, casks, and taps.)
---
Use the Brewfile to install everything
Assuming you put the Brewfile in your home directory:

**brew bundle --file=~/Brewfile**

It will install:

All your previously installed CLI tools (brew install)

GUI apps (brew install --cask)

Taps (custom sources)
