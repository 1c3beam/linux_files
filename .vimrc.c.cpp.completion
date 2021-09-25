set nocompatible              " be iMproved, required
filetype off                  " required

" set the runtime path to include Vundle and initialize
set rtp+=~/.vim/bundle/Vundle.vim
call vundle#begin()
" alternatively, pass a path where Vundle should install plugins
"call vundle#begin('~/some/path/here')

" let Vundle manage Vundle, required
Plugin 'gmarik/Vundle.vim'
"Plugin 'AutoClose'
"Plugin 'justmao945/vim-clang'
Plugin 'raimondi/delimitmate'
"Plugin 'shougo/neocomplete.vim'
"Plugin 'ervandew/supertab'
"Plugin 'AutoComplPop'
Plugin 'lifepillar/vim-mucomplete'
Plugin 'nanotech/jellybeans.vim'
"Plugin 'zchee/deoplete-clang'
Plugin 'rhysd/vim-clang-format'
Plugin 'rip-rip/clang_complete'

call vundle#end()            " required
filetype plugin indent on    " required
colorscheme jellybeans
"deoplete-clang configs
"let g:deoplete#sources#clang#libclang_path='/data/data/com.termux/files/usr/lib/libclang.so'
"let g:deoplete#sources#clang#clang_header='/data/data/com.termux/files/usr/include'

"vim-clang-format configs
let g:clang_format#style_options = {
			\ "AccessModifierOffset" : -4,
			\"AllowShortIfStatementsOnASingleLine" : "true",
			\"AlwaysBreakTemplateDeclarations" : "true",
			\"IndentWidth": 4,
			\"TabWidth": 4,
			\"UseTab": "Always"}
"clang_complete configs
let g:clang_complete_auto=1
let g:clang_complete_copen=1
let g:clang_library_path='/data/data/com.termux/files/usr/lib/libclang.so'

"mucomplete configs
set completeopt+=menuone,noselect
let g:mucomplete#enable_auto_at_startup=1
set noinfercase
set completeopt-=preview


set tabstop=4
set noexpandtab
set softtabstop=4
set shiftwidth=4
set colorcolumn=110
highlight ColorColumn ctermbg=darkgray
autocmd CompleteDone * pclose
map <F5> :w <CR> :!gcc % -o %< && ./%< <CR> 
" To ignore plugin indent changes, instead use:
filetype plugin on
"
" Brief help
" :PluginList       - lists configured plugins
" :PluginInstall    - installs plugins; append `!` to update or just :PluginUpdate
" :PluginSearch foo - searches for foo; append `!` to refresh local cache
" :PluginClean      - confirms removal of unused plugins; append `!` to auto-approve removal
"
" see :h vundle for more details or wiki for FAQ
" Put your non-Plugin stuff after this line

