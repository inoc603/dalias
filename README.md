# dalias
Give aliases to frequently used directory

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
```

For an easier cd command, add the following line to your `.bashrc`, `.zshrc`, or
whatever will be sourced at login:

```bash
alias cdd=". dalias cd"
```

Then you can use `cdd DIR_ALIAS` to quickly navigate to your saved directory.

