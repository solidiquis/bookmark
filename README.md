# Bookmark

I'm a neat freak when it comes to my configs and I never liked having a bunch of `cd` aliases in my shell startup configuration file.

## Installation
`cd` into the directory where you want to place the script and run:
`curl https://raw.githubusercontent.com/solidiquis/bookmark/master/bookmark -o bookmark`

I'd recommend either putting this script in your `$PATH` or source it into your shell's config.

Example in `.zshrc`:
```
source $PATH_TO_SCRIPT/bookmark --source_only
```

## Usage
List bookmarks: `lsbm`
```
$ lsbm
dotfiles=/Users/benjamin/dotfiles
code=/Users/benjamin/Desktop/Code
home=/Users/benjamin
bash_reference=/Users/benjamin/Desktop/Code/Bash
wf=/Users/benjamin/Desktop/Code/Ruby/wefunder
```

Make bookmark: `mkbm <name_of_bookmark>`
```
# Bookmarking your current working directory
$ mkbm my_desktop
desktop added.
```

Jump to bookmark: `jbm <name_of_bookmark>`
```
$ jbm my_desktop
```

Remove bookmark: `rmbm <name_of_bookmark>`
```
$ rmbm my_desktop
```
