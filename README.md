|        |                                                     𝑶𝒓𝒊𝒈𝒊𝒏𝒂𝒍 𝑮𝒓𝒖𝒗𝒃𝒐𝒙                                                     |                                                     𝑮𝒓𝒖𝒗𝒃𝒐𝒙 𝑴𝒂𝒕𝒆𝒓𝒊𝒂𝒍                                                     |
| :----: | :----------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------: |
|  𝒉𝒂𝒓𝒅  |  ![original-hard](https://user-images.githubusercontent.com/37491630/61801994-4072df00-ae1f-11e9-8a3a-cc806393f460.png)  |  ![material-hard](https://user-images.githubusercontent.com/37491630/63072979-02487700-bf16-11e9-88ca-e288c094697b.png)  |
| 𝒎𝒆𝒅𝒊𝒖𝒎 | ![original-medium](https://user-images.githubusercontent.com/37491630/61802005-45379300-ae1f-11e9-91bb-012e058eb906.png) | ![material-medium](https://user-images.githubusercontent.com/37491630/63072977-ffe61d00-bf15-11e9-9fcb-1720b4e6b8b2.png) |
|  𝒔𝒐𝒇𝒕  |  ![original-soft](https://user-images.githubusercontent.com/37491630/61801978-3bae2b00-ae1f-11e9-9b7b-33105484be47.png)  |  ![material-soft](https://user-images.githubusercontent.com/37491630/63072974-feb4f000-bf15-11e9-8b9b-34c5bac2711e.png)  |

The syntax highlighting logic used in this branch is as follows:

- **Red**`#ea6962`: Keyword, Statement, Conditional, Repeat, Exception
- **Orange**`#e78a4e`: StorageClass, Operator, Structure, Label, Title, Tag
- **Yellow**`#e3a84e`: Type, Typedef, Special, SpecialChar
- **Green**`#a9b665`: Method, String, Boolean, Character, Number, Float
- **Aqua**`#89b482`: Function, Constant, Define
- **Blue**`#7daea3`: Identifier
- **Purple**`#d3869b`: Macro, PreProc, Include, PreCondit

# Installation

## Via Plugin Manager

Take [vim-plug](https://github.com/junegunn/vim-plug) for example:

```vim
Plug 'sainnhe/gruvbox-material', { 'branch': 'neosyn' }
```

For better syntax highlighting support, please install [sheerun/vim-polyglot](https://github.com/sheerun/vim-polyglot).

## Manually

1. Clone this repository and checkout this branch `git checkout neosyn`.
2. Copy `/path/to/gruvbox-material/colors/*` to `~/.vim/colors/`
3. To install [airline](https://github.com/vim-airline/vim-airline) theme, copy `/path/to/gruvbox-material/autoload/airline/themes/gruvbox_material.vim` to `~/.vim/autoload/airline/themes/gruvbox_material.vim`
4. To install [lightline](https://github.com/itchyny/lightline.vim) theme, copy `/path/to/gruvbox-material/autoload/lightline/colorscheme/gruvbox_material.vim` to `~/.vim/autoload/lightline/colorscheme/gruvbox_material.vim`

## AUR

There is a package available for Arch Linux users in AUR: [gruvbox-material-neosyn-git](https://aur.archlinux.org/packages/gruvbox-material-neosyn-git/)

# Usage

## Vim

Put this in your vimrc:

```vim
set termguicolors

colorscheme gruvbox-material

" for soft background
colorscheme gruvbox-material-soft

" for hard background
colorscheme gruvbox-material-hard
```

If you want to apply this color scheme temporarily, run this command in vim(**this may cause color broken**):

```vim
:colorscheme gruvbox-material
```

## Airline

To enable [airline](https://github.com/vim-airline/vim-airline) color scheme, put this in your vimrc:

```vim
let g:airline_theme = 'gruvbox_material'
```

To apply it without reloading:

```vim
:AirlineTheme gruvbox_material
```

## Lightline

To enable [lightline](https://github.com/itchyny/lightline.vim) color scheme, put this in your vimrc:

```vim
let g:lightline = {}
let g:lightline.colorscheme = 'gruvbox_material'

" or this line
let g:lightline = {'colorscheme' : 'gruvbox_material'}
```

To apply it without reloading:

```vim
:let g:lightline.colorscheme = 'gruvbox_material'
:call lightline#init()
:call lightline#colorscheme()
```

# Customization

- By default, italic is enabled. To disable italic, add `let g:gruvbox_material_kill_italic=1` to your vimrc.
- By default, bold is enabled in lightline color scheme. To disable bold in lightline color scheme, add `let g:gruvbox_material_lightline_kill_bold=1` to your vimrc.

# Contribution

Check this gist for detailed instructions to hack this color scheme: [hack-color-schemes.md](https://gist.github.com/sainnhe/911f78cbb092ac58c8734c423a464935)

# Related Projects

## Code Editor

- [Visual Studio Code](https://github.com/sainnhe/gruvbox-material-vscode)

## Terminal Emulators

- [Alacritty](https://gist.github.com/kamek-pf/2eae4f570061a97788a8a9ca4c893797)
- [kitty](https://gist.github.com/rsaihe/789829b1e475299b015717813715181a)
- [Tilix](https://gist.github.com/sainnhe/5c44ffcd2465198ced6d80ac57b38b34)
- [Windows Terminal](https://gist.github.com/sainnhe/587a1bba123cb25a3ed83ced613c20c0)

## Other

- [Zsh](https://gist.github.com/sainnhe/f92372e14c59750b6ac8dc927ba9f7fe)
- [Tmux](https://gist.github.com/sainnhe/b8240bc047313fd6185bb8052df5a8fb)

# License

[MIT](./LICENSE) && [Anti-996](./Anti-996-LICENSE)
