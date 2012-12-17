# Gnome Grabbox

It's a tool to provide [grabbox](http://grabbox.devsoft.no/) functionality on linux, in gnome environment.

Basicly it takes care of 

* saving screenshots to a dropbox public folder
* with random names
* shorten the public url of that screenshot
* then copy this short url to clipboard

The random names and the shotened url features are optional in grabbox, but burned-in in this script.

## How to install

Clone this repo in your home directory

```shell
cd ~
git clone https://github.com/miklos-martin/.gnome-grabbox.git
# You probably will have to make the script executable
chmod +x ~/.gnome-grabbox/capture
```
Make a keyboard shortcut which runs the `~/.gnome-grabbox/capture`

You're done!

**NOTE** You should clone it to your home dir, with that exact name.
It's in an early state of development, and has some paths burned in the code.

They might be cleaned out in the future.

## Dependencies

Among gnome and python, you must have [Dropbox](https://www.dropbox.com/downloading?os=lnx), and the [Dropbox CLI](http://www.dropboxwiki.com/Using_Dropbox_CLI) installed.
**NOTE** The path of your Dropbox public folder, and of the `dropbox.py` is also burned in for now. They are `~/Dropbox` and `~/bin/dropbox.py`. These are the paths by default.
Other dependencies: xclip.

## Debugging

If you notice, that this script doesn't do anything, try run it from a terminal. You may have unmet dependencies, or other paths.

## Usage

1. Take a screenshot with the chosen keyboard shortcut.
2. You might have to wait for a second or two, while dropbox finishes the upload.
3. The short URL of your fresh screenshot will be on your clipboard.

----

If you want to use it in other environments, please send a pull request on a new branch.
