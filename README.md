# Some git stuff

### How?

In your favourite text editor open the .gitconfig file located in `~/.gitconfig` and just copy pasta the contents from `.gitconfig-aliases` into it.

For the bash sub commands, either copy or download the files in this repos `.local/bin` and put them in `~/.local/bin` and make them all executable with something like `chmod +x ~/.local/bin/*` (just be careful you dont have weird shit in here, i recommend otherwise to make them executable one at a time)

then in your `bashrc` or `zshrc` (or `config.nu` or whatever shell you use) add this to the file `export PATH="$HOME/.local/bin:$PATH"` to make the files recognizable by the Git CLI.

### how to use `sus` and `branches recent`

Simply just use the command `git sus` or `git branches recent` in a valid git initialized directory.

For `git sus` you have some options, like `git sus --since="5 days ago"` to get your commits from the last 5 days. By default, `git sus` will show you your last commits from yesterday.
