# cwv
Course web-page viewer (`cwv`) is a command-line tool for viewing washu engineering department course web-pages.

`cwv` uses `w3m` to dump the webpage in a human readable format and `less` to display the webpage.

## How to import
To use `cwv`, you will first need to install `w3m` and `less` from your package manager.

`less` comes pre-installed on raspberry pi os, and one can install `w3m` by running `sudo apt-get install w3m`.

Then import `cwv` by simply running `source cwv`. If you wish, you may add this to `~/.bashrc` or `~/.zshrc`.

## How to use
```
cwv class [folder] [page]
```
This will present the url "https://classes.engineering.wustl.edu/class/folder/page"
