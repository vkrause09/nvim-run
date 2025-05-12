A minimal Neovim plugin that opens a floating terminal to run the current file based on its filetype.

## Supported Languages

- Python
- Lua
- JavaScript / TypeScript
- Shell
- Go
- C / C++

## Installation

Using [lazy.nvim]

```lua
{
  "vkrause09/nvim-run",
  config = function()
    vim.keymap.set("n", "<leader>r", require("nvim-run").run_current_file, { desc = "Run file in floating terminal" })
  end
}
```

Using [packer.nvim]

```lua
{
    use ("vkrause09/nvim-run")
}
