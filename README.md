# .vimrc file for iVim

iVim is a text editing app for iOS devices. It is a clone of Vim 8.1 -- it is **not** a clone of Neovim.

Because iVim is a clone of Vim, it lacks the extensibility of a Vim client on a Linux terminal. Therefore, this repo is a modified set of Vim dotfiles that *will* work on iVim. The features that only work on "real Vim" have been commented out or removed.

## Instructions

iVim has a working directory contained within the "On My iPad" location in the Files app.

The '.vim' directory within the repo should be downloaded and added to the 'iVim' folder.

In addition, the plugins that work on iVim need to be copied and pasted into the '.vim/bundle' directory. The plugins that work on iVim are those that are written in Vimscript. However, not all Vimscript plugins work (example: FZF).

Actively used plugin list:
- ctrlpvim/ctrlp.vim
- vim-airline/vim-airline
- vimwiki/vimwiki

Some plugins are hardcoded, mainly because they do not reside in the '.vim/bundle' directory. Those plugins are the following:
- tpope/vim-pathogen
- tpope/vim-surround

## Thoughts

Look into:
- is there a way to perform `git` commands on iPad?
    - any way to clone repos from the iPad itself? directly into iVim directory?
- plugin = Donaldttt/fuzzyy
    - functions similar to telescope on Neovim
    - includes a preview pane
    - has a Vim8 branch
    - as of 2023 Nov 16, Vim8 branch does ***not*** work with iVim
