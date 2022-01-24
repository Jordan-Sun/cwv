# cwv
Course web-page viewer (`cwv`) is a command-line tool for viewing washu engineering department course web-pages.

`cwv` uses `w3m` to dump the webpage in a human readable format and `less` to display the webpage.

## Alternatives
Consider using lynx and add `alias lclass="lynx https://classes.engineering.wustl.edu/class"`, replacing class with the class name, to your `./bash_aliases`.
Alternatively, add the following function that takes the class name as an argument
```
lcw() {
     lynx "https://classes.engineering.wustl.edu/$1"
}
```

## How to use

To use `cwv`, you will first need to install `w3m` and `less` from your package manager.

On Raspberry Pi OS, `less` comes pre-installed and one can install `w3m` by running `sudo apt-get install w3m`.

To run `cwv`, simply type
```
cwv class [folder] [page]
```
This will present the url "https://classes.engineering.wustl.edu/class/folder/page"

If you wish, you can add `cwv` to your `/bin` folder.
