# .vimrc for YAML

Add this line into your `$HOME/.vimrc` configuration file:

```.vimrc
autocmd FileType yaml setlocal ai ts=2 sw=2 et
```

and it will make editing YAML files with `vim` easier - pressing `<TAB>` will make exactly 2 spaces (not tab).
