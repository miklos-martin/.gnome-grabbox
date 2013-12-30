# Gnome Grabbox

It's a tool to provide [grabbox](http://grabbox.devsoft.no/) functionality on linux, in gnome environment.

Basicly it takes care of 

* saving screenshots to a dropbox public folder
* with random names
* shorten the public url of that screenshot
* then copy this short url to clipboard

The random names and the shortened url features are optional, see the [configuration sample](https://github.com/miklos-martin/.gnome-grabbox/blob/master/config.sample).

## How to install

`curl -L https://raw.github.com/miklos-martin/.gnome-grabbox/master/install | sh`

or

`wget --no-check-certificate https://raw.github.com/miklos-martin/.gnome-grabbox/master/install -O - | sh`

Or you can do it manually

```shell
cd ~
git clone https://github.com/miklos-martin/.gnome-grabbox.git
cp .gnome-grabbox/config.sample .gnome-grabbox.conf
```

Make a keyboard shortcut which runs the `/full/path/to/your/homedir/.gnome-grabbox/capture`

You're done!

## Configuration

See the [configuration sample](https://github.com/miklos-martin/.gnome-grabbox/blob/master/config.sample)

## Dependencies

* [Dropbox](https://www.dropbox.com/downloading?os=lnx)
* [Dropbox CLI](http://www.dropboxwiki.com/Using_Dropbox_CLI)
* [xclip](http://manpages.ubuntu.com/manpages/precise/man1/xclip.1.html)

## Debugging

If you notice, that this script doesn't do anything, try run it from a terminal. You may have unmet dependencies, or you need to customize the paths of dropbox stuffs. See the [configuration sample](https://github.com/miklos-martin/.gnome-grabbox/blob/master/config.sample).

## Usage

1. Take a screenshot with the chosen keyboard shortcut.
2. You might have to wait for a second or two, while dropbox finishes the upload.
3. The short URL of your fresh screenshot will be on your clipboard.

----

If you want to use it in other environments, please send a pull request on a new branch.
