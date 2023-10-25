# .vimrc file for iVim

iVim is a text editing app for iOS devices. It is essentially a Vim clone, but does not claim to be a Neovim clone.

This repo is an experiment to see how much iVim can do.

## Instructions

iVim has a working directory contained within the "On My iPad" location in the Files app.

This repo can either replace the "iVim" folder in "On My iPad," or the contents of this repo can be copied and pasted into the "iVim" folder.

In addition, the plugins that work on iVim need to be copied and pasted into the '.vim/bundle' directory. The plugins that work on iVim are those that are written in Vimscript. However, not all Vimscript plugins work (example: FZF).

Actively used plugin list:
- vim-airline/vim-airline
- vimwiki/vimwiki

Some plugins are hardcoded, mainly because they do not reside in the '.vim/bundle' directory. Those plugins are the following:
- tpope/vim-pathogen
- tpope/vim-surround

## Thoughts

Look into:
- is there a way to perform `git` commands on iPad?
    - any way to clone repos from the iPad itself? directly into iVim directory?
