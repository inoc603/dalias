# dalias

Give aliases to frequently used directory

Unlike autojump, you have to add the directory to dalias yourself. Despite the
extra setup, you get more accurate jumps, and you can name your directories as
you like. This is very useful when you want to jump to directory with randomly
generated names.

## Install

Put the `dalias` script anywhere in your `PATH` so you can find it.

## Usage

Basic usage:

```bash
# save current directory with custom alias
$ dalias save foo

# list saved aliases
$ dalias ls
foo /home/me/nested/dir/hard/to/navigate

# cd to saved directory
$ . dalias cd foo

# remove alias
$ dalias rm foo

# clean aliases to non-existing folder
$ dalias clean
```

For an easier cd command, add the following line to your `.bashrc`, `.zshrc`, or
whatever will be sourced at login:

```bash
alias cdd=". dalias cd"
```

Then you can use `cdd DIR_ALIAS` to quickly navigate to your saved directory.

