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

  set number
  set colorcolumn=80

  let g:UltiSnipsExpandTrigger           = '<tab>'
  let g:UltiSnipsJumpForwardTrigger      = '<tab>'
  let g:UltiSnipsJumpBackwardTrigger     = '<s-tab>'
  let g:ycm_key_list_select_completion   = ['<C-j>', '<C-n>', '<Down>']
  let g:ycm_key_list_previous_completion = ['<C-k>', '<C-p>', '<Up>']

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

[YouCompleteMe](https://github.com/Valloric/YouCompleteMe)

[Numbers](https://github.com/myusuf3/numbers.vim)

## REACT ##

[react-redux-links](https://github.com/markerikson/react-redux-links)

[react-redux-links - redux-architecture](https://github.com/markerikson/react-redux-links/blob/master/redux-architecture.md)

[Boilerplates and Starter Kits - beginner](https://github.com/facebookincubator/create-react-app)

[Boilerplates and Starter Kits - Full-Featured](https://github.com/davezuko/react-redux-starter-kit)


## React Native ##

[React Native](https://github.com/facebook/react-native)
[react-native-redux-starter-kit](https://github.com/LeoLeBras/react-native-redux-starter-kit)
[React Native Seed](https://github.com/GeekyAnts/react-native-boilerplate-redux-typescript)

## REACT On RAILS ##

[ReactOnRails](https://github.com/shakacode/react_on_rails)

#### Installing ####


1. New Rails app: rails new my-app --webpack=react. cd into the directory.
2. Add gem version: gem 'react_on_rails', '~> 9.0.1'
3. Run the generator: rails generate react_on_rails:install --redux
4. Start the app: rails s
5. Visit http://localhost:3000/hello_world
## Setup new Mac ##
1. install apps
- Chrome -> set default
- vivify
- twist
- toggle
- slack
- authy
- iterm2 ( setup theme )

2. Install codeing
- brew: https://brew.sh/

- git: `brew install git`

- ssh: `ssh-keygen -t ed25519 -C “xx”`

- tmux: `brew install tmux`

- vim: https://github.com/remitano/janus-plus-oss

- python:
  `brew install python3`
  echo "alias pip=pip3" >> ~/.zprofile

- neovim:
  `brew install neovim`
  echo "alias vim=nvim" >> ~/.zprofile

- asdf:
  `brew install coreutils curl git`
  `brew install asdf`
  echo ". /opt/homebrew/opt/asdf/libexec/asdf.sh" >> ~/.zprofile
  `asdf plugin add nodejs https://github.com/asdf-vm/asdf-nodejs.git`
  `asdf install nodejs 20.0.0`
  `asdf global nodejs latest`
  `brew install gpg gawk`
  echo 'PATH="/opt/homebrew/opt/gawk/libexec/gnubin:$PATH"' >> ~/.zprofile

- tig

```
brew install tig
```

## Setup new Mac ##
1. install apps
- Chrome -> set default
- vivify
- twist
- toggle
- slack
- authy
- iterm2 ( setup theme )

2. Install coding
- brew: https://brew.sh/

- git:

  ```
  brew install git
  ```

- Oy my zssh

  ```
  sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
  ```



- ssh:

  ```
  ssh-keygen -t ed25519 -C “youremail@email.com”
  ```



- Ack

  ```
  brew install ack
  ack --create-ackrc >> ~/.ackrc
  ```

- tmux:

  ```
  brew install tmux
  ```

- vim: https://github.com/remitano/janus-plus-oss

  - fix LeaderF

    ```
    pip3 install --user --upgrade neovim
    ```

    

- python:

  ```
  brew install pyenv
  pyenv install 2.7.18
  pyenv install 3.9.10
  pyenv global 3.9.10
  pyenv versions
  ```

- neovim:
  ````
  brew install neovim
  echo "alias vim=nvim" >> ~/.zprofile
  ````

- asdf:
```
brew install coreutils curl git
brew install asdf
echo ". /opt/homebrew/opt/asdf/libexec/asdf.sh" >> ~/.zprofile
```
```
asdf plugin add ruby https://github.com/asdf-vm/asdf-ruby.git
asdf plugin add nodejs https://github.com/asdf-vm/asdf-nodejs.git
asdf install nodejs 20.0.0
asdf global nodejs latest
brew install gpg gawk
echo 'PATH="/opt/homebrew/opt/gawk/libexec/gnubin:$PATH"' >> ~/.zprofile
```
- tig:
```
brew install tig
```

- Dot files:

```
curl https://raw.githubusercontent.com/tanna88/tannauit.github.io/master/dotfiles/.tmate.conf --output ~/.tmate.conf
curl https://raw.githubusercontent.com/tanna88/tannauit.github.io/master/dotfiles/.tmux.conf --output ~/.tmux.conf
curl https://raw.githubusercontent.com/tanna88/tannauit.github.io/master/dotfiles/.vimrc.after --output ~/.vimrc.after
```

- Development

  ```
  brew install postgresql@11
  echo 'export PATH="/opt/homebrew/opt/postgresql@11/bin:$PATH"' >> ~/.zprofile
  export LDFLAGS="-L/opt/homebrew/opt/postgresql@11/lib"
  export CPPFLAGS="-I/opt/homebrew/opt/postgresql@11/include"
  brew services restart postgresql@11
  ```

  ```
  brew install redis
  brew services start redis
  ```

  ```
  brew install memcached
  brew services restart memcached
  ```

  ```
  brew install imagemagick
  ```



3. Install project

- Notes for M2
  - Required notejs version 14.16 or above

some dependencies

```
brew install haproxy
npm install -g yarn
```

```
pyenv install 2.7.18
pyenv install 3.9.10
pyenv global 2.7.18
pyenv shims
asdf install
gem install bundler
```

```
curl https://raw.githubusercontent.com/tanna88/tannauit.github.io/master/dotfiles/.bundle/config --output ~/.bundle/config
```

Remember update correct key in bundle config

- fix installing PG error

  ```
  brew install libpq
  gem install pg -v '1.2.3' --user-install -- --with-pg-config=/opt/homebrew/Cellar/libpq/15.2/bin/pg_config
  ```

- Fix openssl

  ```
  brew install openssl@1.1
  ```

  check version by try cd to

  ```
  cd /opt/homebrew/Cellar/openssl@1.1
  cd tab & enter
  cd tab & enter
  pwd
  ```

  EX: the output /opt/homebrew/Cellar/openssl@1.1/1.1.1t/lib

  ```
  ln -s /opt/homebrew/Cellar/openssl@1.1/1.1.1t/lib/libssl.1.1.dylib /usr/local/lib/libssl.so.1.0.0.dylib
  ln -s /opt/homebrew/Cellar/openssl@1.1/1.1.1t/lib/libcrypto.1.1.dylib /usr/local/lib/libcrypto.1.0.0.dylib
  ```
- Fix rgrpc error

  ```
  bundle config set force_ruby_platform true
  gem uninstall -aIx
  bundle install
  ```

- Fix can not install puppeteer

  ```text
  brew install chromium
  ```
