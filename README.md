# .vimrc file for iVim

iVim is a text editing app for iOS devices that brings Vim motions to Apple hardware. It is a clone of Vim 8.1.

However, because iVim is not a perfect clone, it lacks the extensibility of a Vim client on a Linux terminal. Therefore, this repo is a modified set of Vim dotfiles that *will* work on iVim. The features that only work on "real" Vim have been commented out or removed.

This repo is being modified to work as both a Vim and iVim config interchangeably.

## Instructions

iVim has a working directory contained within the "On My iPad" location in the Files app.

The '.vim' directory within the repo should be downloaded and added to the 'iVim' folder.

## iVim & Vim

The main difference between iVim and "real" Vim is the package manager. iVim has a built-in package manager, for a fee. Otherwise, `pathogen` is a preferable option.

To an extent, it's possible to work around this by incorporating "hardcoded" plugins and themes. This works best when the package is a single file that doesn't change much. The same is true for theme packages. The themes that have been hardcoded, unless specified, are those composed of only a single file.

## Plugins

The following are plugins that have been hardcoded with no issues:
- jiangmiao/auto-pairs
- tpope/vim-pathogen
- tpope/vim-surround

The following are plugins that have not been hardcoded, and therefore require manual installation into the '.vim/bundle' directory:
- ctrlpvim/ctrlp.vim
- donaldttt/fuzzyy (doesn't work on iVim)
- vim-airline/vim-airline
- vimwiki/vimwiki

## Themes

The following are themes that have been hardcoded with no issues:
- connorholyday/vim-snazzy
- itsjunetime/rose-pine-vim
- NLKNguyen/papercolor-theme
- raphamorim/lucario
- rose-pine/vim

The following are themes that have been hardcoded, despite having airline themes in their '.vim/autoload' directories:
- artanikin/vim-synthwave84
- ayu-theme/ayu-vim
- ghifarit53/tokyonight-vim
- lifepillar/vim-gruvbox8
- morhetz/gruvbox
- thedenisnikulin/vim-cyberpunk

The following themes only work properly when installed to the '.vim/bundle' directory:
- joshdick/onedark.vim
- sainnhe/gruvbox-material

## Thoughts

Look into:
- plugin = Donaldttt/fuzzyy
    - functions similar to telescope on Neovim
        - includes a preview pane
    - has a Vim8 branch
        - as of 2023 Nov 16, Vim8 branch does ***not*** work with iVim

## Current notes

Whether using iVim or Vim, attempt a `:PlugInstall` when first running the text editor. If plug.vim doesn't work, remove the file and clone plugins into the '.vim/bundle' directory.
