# .vimrc file for iVim

iVim is a text editing app for iOS devices. It is a clone of Vim 8.1 -- it is **not** a clone of Neovim.

Because iVim is a clone of Vim, it lacks the extensibility of a Vim client on a Linux terminal. Therefore, this repo is a modified set of Vim dotfiles that *will* work on iVim. The features that only work on "real Vim" have been commented out or removed.

## Instructions

iVim has a working directory contained within the "On My iPad" location in the Files app.

The '.vim' directory within the repo should be downloaded and added to the 'iVim' folder.

## iVim & Vim

iVim is not Vim, though it is close. This repo is being modified to work as both a Vim and iVim config interchangeably.

The main issue is the package manager. iVim has a paid for package manager. To an extent, it's possible to work around this by incorporating "hardcoded" plugins and themes. This works best when the package is a single file that doesn't change much.

The following are plugins that have been hardcoded:
- tpope/vim-pathogen
- tpope/vim-surround

The following are plugins that have not been hardcoded, and therefore require manual installation into the '.vim/bundle' directory:
- ctrlpvim/ctrlp.vim
- donaldttt/fuzzyy (doesn't work on iVim)
- vim-airline/vim-airline
- vimwiki/vimwiki

The same is true for theme packages. The themes that have been hardcoded, unless specified, are those composed of only a single file.

The following are plugins that have been hardcoded:
- connorholyday/vim-snazzy
- itsjunetime/rose-pine-vim
- NLKNguyen/papercolor-theme
- raphamorim/lucario
- rose-pine/vim

The following are plugins that have been hardcoded, despite having airline themes in the '.vim/autoload' directory:
- artanikin/vim-synthwave84
- ayu-theme/ayu-vim
- ghifarit53/tokyonight-vim
- joshdick/onedark.vim (doesn't load properly without other files)
- lifepillar/vim-gruvbox8
- morhetz/gruvbox
- sainnhe/gruvbox-material (doesn't load properly without other files)
- thedenisnikulin/vim-cyberpunk

Potentially, the themes with more than 1 file can also be added to the '.vim/bundle' directory.

## Thoughts

Look into:
- is there a way to perform `git` commands on iPad?
    - any way to clone repos from the iPad itself? directly into iVim directory?
    - app called 'Working Copy'
- plugin = Donaldttt/fuzzyy
    - functions similar to telescope on Neovim
    - includes a preview pane
    - has a Vim8 branch
    - as of 2023 Nov 16, Vim8 branch does ***not*** work with iVim
