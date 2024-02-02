# Neovim Personal Notes

### Temporary Fix for the Json files

#### Formatting - File unrecognized

When you open a json file and if tree-sitter doesn't recognize it as a json file, you can use the command `:set filetype=json` for neovim to start formatting it.

#### Conceal

The reason why you see the json commands in the config files without `" "` and when you move your cursor line to a line, and see `" "` appear, it is because you have your neovim `opt.conceallevel` set to 2 or 3 also it depends on `cursorconceal` settings. You may need that setting for some plugins such as indent or markdown. To fix the issue in json file, you should execute `setlocal conceallevel=0` and it will fix it.
