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

## REACT ##

[react-redux-links](https://github.com/markerikson/react-redux-links)

[react-redux-links - redux-architecture](https://github.com/markerikson/react-redux-links/blob/master/redux-architecture.md)

[Boilerplates and Starter Kits - beginner](https://github.com/facebookincubator/create-react-app)

[Boilerplates and Starter Kits - Full-Featured](https://github.com/davezuko/react-redux-starter-kit)



## REACT On RAILS ##

[ReactOnRails](https://github.com/shakacode/react_on_rails)

#### Installing ####


1. New Rails app: rails new my-app --webpack=react. cd into the directory.
2. Add gem version: gem 'react_on_rails', '~> 9.0.1'
3. Run the generator: rails generate react_on_rails:install --redux
4. Start the app: rails s
5. Visit http://localhost:3000/hello_world
