Build vim editor in Linux into an effective C++ programming IDE
===============================================

- [Intro](#intro)
- [Installation](#installation)
- [Included Plugins](#included-plugins)
- [Key Mappings](#key-mappings)
    - [Basic mappings](#basic-mappings)
        - [Normal mode mappings](#normal-mode-mappings)
        - [Insert mode mappings](#insert-mode-mappings)
        - [Visual mode mappings](#visual-mode-mappings)
    - [Plugins mappings](#plugins-mappings)
        - [Normal mode mappings](#normal-mode-mappings-1)
        - [Insert mode mappings](#insert-mode-mappings-1)
        - [Visual mode mappings](#visual-mode-mappings-1)

Intro
-----

可能这是最简单的将 vim 构建为 IDE 的项目。

Installation
-----

1. Download plug.vim and put it in the "autoload" directory.

        curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
            https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim

2. Download this vimrc and put it in the ~/ directory.


3. Install Plugins.

        vim +PlugInstall +qall

4. Finished! Enjoy it.

Included Plugins
-----

I think you should read the docs of these plugins to use them efficiently.

- [vim-plug](https://github.com/junegunn/vim-plug): Minimalist Vim Plugin Manager
- [vim-easy-align](https://github.com/junegunn/vim-easy-align): A Vim alignment plugin
- [vim-colors-solarized](https://github.com/altercation/vim-colors-solarized): precision colorscheme for the vim text editor
- [vim-tomorrow-theme](https://github.com/chriskempson/vim-tomorrow-theme): Tomorrow Theme for Vim
- [ultisnips](https://github.com/SirVer/ultisnips): The ultimate snippet solution for Vim
- [vim-multiple-cursors](https://github.com/terryma/vim-multiple-cursors): True Sublime Text style multiple selections for Vim
- [vim-move](https://github.com/matze/vim-move): Plugin to move lines and selections up and down
- [vim-indent-guides](https://github.com/nathanaelkane/vim-indent-guides): A Vim plugin for visually displaying indent levels in code
- [vim-fswitch](https://github.com/derekwyatt/vim-fswitch): Vim plug for switching between companion source files (e.g. ".h" and ".cpp")
- [vim-protodef](https://github.com/derekwyatt/vim-protodef): Vim plugin for pulling in C++ function prototypes into implementation files
- [nerdcommenter](https://github.com/scrooloose/nerdcommenter): Vim plugin for intensely orgasmic commenting
- [nerdtree](https://github.com/scrooloose/nerdtree): A tree explorer plugin for vim
- [tagbar](https://github.com/majutsushi/tagbar): Vim plugin that displays tags in a window, ordered by scope
- [vim-polyglot](https://github.com/sheerun/vim-polyglot): A solid language pack for Vim
- [syntastic](https://github.com/scrooloose/syntastic): Syntax checking hacks for vim
- [minibufexpl.vim](https://github.com/fholgado/minibufexpl.vim): Elegant buffer explorer - takes very little screen space
- [gundo.vim](https://github.com/sjl/gundo.vim): Gundo.vim is Vim plugin to visualize your Vim undo tree
- [ctrlsf.vim](https://github.com/dyng/ctrlsf.vim): An ack.vim alternative mimics Ctrl-Shift-F on Sublime Text 2
- [ctrlp.vim](https://github.com/kien/ctrlp.vim): Fuzzy file, buffer, mru, tag, etc finder
- [vim-instant-markdown](https://github.com/suan/vim-instant-markdown): Instant Markdown previews from VIm
- [YouCompleteMe](https://github.com/Valloric/YouCompleteMe): A code-completion engine for Vim

Key Mappings
-----

The `<leader>` key is `;`

### Basic mappings

#### Normal mode mappings

- `;w` Write (save) the file, but don't exit
- `;q` Quit
- `;Q` Quit and throw away changes
- `;p` Paste
- `;hw` Jump to the left window
- `;jw` Jump to the down window
- `;kw` Jump to the up window
- `;lw` Jump to the right window
- `<tab>` Jump to the next window
- `<S-tab>` Jump to the previous window
- `]q` Jump to next record/match in quickfix list
- `[q` Jump to previous record/match in quickfix list
- `<F8>` Change color scheme
- `<F11>` Fullscreen

#### Insert mode mappings

- `<C-s>` Write (save) the file, but don't exit
- `<C-h>` Move left
- `<C-j>` Move down
- `<C-k>` Move up
- `<C-l>` move right

#### Visual mode mappings

- `;y` Copy

### Plugins mappings

#### Normal mode mappings

- `;fs` Switch between companion source files (e.g. ".h" and ".cpp")
- `<F2>` Toogle Tagbar visible
- `<F3>` Toogle NERD-Tree visible
- `<F4>` Toogle minibufexpl visble
- `]b` Jump to the next buffer 
- `[b` Jump to the previous buffer 
- `;ud` Toggle Gundo visible 
- `<C-f>` Search and split a new window to show search result
- `<C-p>` Open ctrlp window (alternative :CtrlP)
- `;md` Launch the preview window for current markdown file
- `;jc` Go to declaration
- `;jd` Go to definition

#### Insert mode mappings

- `<F2>` Toogle Tagbar visible
- `<F3>` Toogle NERD-Tree visible
- `<F4>` Toogle minibufexpl visble

#### Visual mode mappings

- `<C-k>` Move current line/selections up
- `<C-j>` Move current line/selections down
