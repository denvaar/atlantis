# Atlantis
#### Vim color scheme

### Manual Installation (Neovim)

1. Add `atlantis.vim` to `/colors`
2. Add the following to `init.vim`

```
if (has("termguicolors"))
  set termguicolors
endif
let g:atlantis_italics_enabled="1"
colorscheme atlantis
```

3. If you would like syntax highlighting for React, you will have to modify the default XML syntax highlighting. Create or edit `/after/syntax/xml.vim` and add the following code:
```
syn region xmlTagName matchgroup=xmlEndTag start=+</+ end=+>+
```

### Vundle Installation

TODO
