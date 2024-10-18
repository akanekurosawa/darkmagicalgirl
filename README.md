# DISCLAIMER

**IF YOU'RE READING THIS, THIS IS JUST A RENAMED COPY OF THE ORIGINAL FORK. USE THAT ONE INSTEAD!**

### About

A mildly modified, delightfully dark fork of tokyodark.nvim inspired by Sailor Moon and the Star Guardians.

### Features

### Installation

Install with your favorite package manager:

[lazy](https://github.com/folke/lazy.nvim)

``` lua
{
    "akanekurosawa/darkmagicalgirl",
    lazy = false,
    priority = 1000,
    opts = {
        -- custom options here
    },
    config = function(_, opts)
        require("darkmagicalgirl").setup(opts) -- calling setup is optional
        vim.cmd [[colorscheme darkmagicalgirl]]
    end,
}
```

### Default configuration

```lua
local default_config = {
    transparent_background = false, -- set background to transparent
    gamma = 1.00, -- adjust the brightness of the theme
    styles = {
        comments = { italic = true }, -- style for comments
        keywords = { italic = true }, -- style for keywords
        identifiers = { italic = true }, -- style for identifiers
        functions = {}, -- style for functions
        variables = {}, -- style for variables
    },
    custom_highlights = {} or function(highlights, palette) return {} end, -- extend highlights
    custom_palette = {} or function(palette) return {} end, -- extend palette
    terminal_colors = true, -- enable terminal colors
}
```

### Inspiration

- [tokyodark.nvim](https://github.com/tiagovla/tokyodark.nvim)
- [tokyonight-vim](https://github.com/ghifarit53/tokyonight-vim)
- [tokyo-night-vscode-theme](https://github.com/enkia/tokyo-night-vscode-theme)
