# La mia configurazione di VIM


In questo repository ho messo il mio file .vimrc e i plugin che uso. In particolare, sono inclusi i seguenti plugin:

    - SimpylFold (code folding)
    - Jedi-Vim (auto-completition)
    - vim-python-PEP8-indent (indentation)
    - Syntastic (syntax highlight)
    - Cucci Theme (color theme)
    - NerdTree (files tree)
    - NerdCommenter (commentare in blocco delle righe)
    - ctrlp.vim (handle multiple files)
    - vim-fugitive (Git wrapper)
    - powerline (enhanced status line)
    - vim-signify (vari diffs)
    - vim-startify (spash screen - NB. me lo sono personalizzato)
    - vim-gitgutter (git diffs)
    - tagbar (class tree, necessita di exuberant ctags)


In più, sono state definite queste scorciatoie da tastiera:

  - &lt;space&gt; Folding
  - &lt;F9&gt; Chiudi tutto (folding)
  - &lt;F10&gt; Apri tutto (folding)
  - &lt;C-J&gt; Spostanti nel buffer a destra
  - &lt;C-K&gt; Spostati nel buffer in alto
  - &lt;C-L&gt; Spostati nel buffer in basso
  - &lt;C-H&gt; Spostati nel buffer a sinistra
  - &lt;C-n&gt; Mostra alberatura
  - &lt;F5&gt; Salva ed esegui con Python
  - &lt;F3&gt; Apre un nuovo buffer a destra con split verticale
  - &lt;F8&gt; Mostra alberatura classi
 
Altre definizioni:

```vim
" Python - PEP 8
au BufNewFile,BufRead *.py
\ set tabstop=4 |
\ set softtabstop=4 |
\ set shiftwidth=4 |
\ set textwidth=79 |
\ set expandtab |
\ set autoindent |
\ set fileformat=unix
 
" Full Stack
au BufNewFile,BufRead *.js, *.html, *.css
\ set tabstop=2 |
\ set softtabstop=2 |
\ set shiftwidth=2 |
```

Installazione
-------------
  - Clona questo repo, metti tutto dentro .vim e il file .vimrc in ~/
  - Installa Vundle:


```bash
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```

  - Installa exuberant ctags, e con pip install: jedi, pyflakes
  - Entra in vim ed esegui :PluginInstall
  - Installa i font per Powerline con:

```bash
git clone https://github.com/powerline/fonts.git
cd fonts
./install.sh
```

ScreenShots
-----------
![alt tag](intro.png)
![alt tag](dev.png)

License
----

MIT


**Free Software, Hell Yeah!**
