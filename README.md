`README.md` Tannauit

## VIMRC ##
Install the basic from https://github.com/amix/vimrc

Then I add following config

	"CUSTOME FROM HERE"
	"=============="
	
	"GENERAL"
	"=============="
	execute pathogen#infect()
	let mapleader = "\<Space>"
	autocmd BufWritePre * %s/\s\+$//e
	nmap <leader>w :w!<CR>
	"PWD"
	map <leader>cd :cd %:p:h<cr>:pwd<cr>
	"TAB helper"
	map <leader>tn :tabnew<cr>
	map <leader>to :tabonly<cr>
	map <leader>tc :tabclose<cr>
	map <leader>tm :tabmove
	"COPY to clipboard"
	set clipboard+=unnamed
	vmap <C-c> "+yi
	vmap <C-x> "+c
	vmap <C-v> c<ESC>"+p
	imap <C-v> <ESC>"+pa
	"=============="
	"
	"THEME"
	"=============="
	syntax enable
	set background=dark
	let g:solarized_termcolors=256
	colorscheme solarized
	"=============="
	
	"MRU"
	"============"
	map <leader>f :MRU<CR>
	"============"
	
	"NERDTREE"
	"============"
	map <C-n> :NERDTreeToggle<CR>
	"============"
	
	"CtrP"
	"============"
	let g:ctrlp_map = '<c-p>'
	"============"
	
	"ACK"
	"============"
	map <leader>g :Ack
	"============"
	
	"yankStack"
	"============"
	call yankstack#setup()
	let g:yankstack_map_keys = 0
	nmap <leader>p <Plug>yankstack_substitute_older_paste
	nmap <leader>P <Plug>yankstack_substitute_newer_paste
	"============"

I recommend you should read one by one plugin to understand how it work before using it.

---
There are some plugins that I install for my vim

[ack.vim](https://github.com/mileszs/ack.vim)

[mru.vim](https://github.com/vim-scripts/mru.vim)

[vim-fugitive.vim](https://github.com/tpope/vim-fugitive)

[clever-f.vim](https://github.com/rhysd/clever-f.vim)

[nerdtree](https://github.com/scrooloose/nerdtree)

[vim-rails.vim](https://github.com/tpope/vim-rails)

[ctrlp.vim](https://kien.github.com/ctrlp.vim)

[vim-colors-solarized](https://github.com/altercation/vim-colors-solarized)

[vim-yankstack.vim](https://github.com/maxbrunsfeld/vim-yankstack)