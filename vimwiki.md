# Vimwiki
* Configuration:
```lua
vim.g.vimwiki_list = {
  {
    path = '~/Dropbox/vimwikiz',
    syntax = 'markdown',
    ext  = '.md',
    diary_frequency = 'daily',
    markdown_link_ext = 1,
  },
  {
    path = '~/Dropbox/vimwikiz/tech',
    syntax = 'markdown',
    ext  = '.md',
    diary_frequency = 'daily',
    diary_rel_path = "../diary/",
    markdown_link_ext = 1,
  },
  {
    path = '~/Dropbox/vimwikiz/entertainment',
    syntax = 'markdown',
    ext  = '.md',
    diary_frequency = 'daily',
    diary_rel_path = "../diary/",
    markdown_link_ext = 1,
  },
  {
    path = '~/Dropbox/vimwiki',
    syntax = 'markdown',
    ext  = '.md',
    diary_frequency = 'weekly',
    markdown_link_ext = 1,
  }
}
```


## Commands
* Opening the wiki:
  * `<leader>ww` opens the main wiki
  * The nested wikis can be navigated to but also opened:
    * `2<leader>ww` for tech, etc.

### Creating a new page
* Keymap:
  * `keymap('n', '<leader>n', ':VimwikiGoto ', {})`
* Navigate to the subwiki you want to create and then `<leader>n`


## Telescope integration
* `use 'codevion/telescope-vimwiki.nvim'`



