# Xdebug Toggler for OSX

>> This script is inspired by the [w00fz][xdebug-osx]

[Xdebug][xdebug] is a must have extension for PHP, although the times you don't actually need it, it's a drag.

This simple script allows to toggle `on` and `off` [Xdebug][xdebug] and is meant for anyone running `PHP` and `Xdebug` installed via [Homebrew][brew].

You can follow the _OS X Apache Setup_ guide, divided in two parts, to get the perfect MAMP setup on OSX:

## Quick Installation

```
curl -L https://raw.githubusercontent.com/sourcebroker/tools/master/xdebug-toggle/xdebug-toggle > /usr/local/bin/xdebug-toggle
```

## Installation with clone

```
git clone git@github.com:sourcebroker/tools.git
```

Add `/usr/local/bin` to your `$PATH`. If you use the Bash shell, you can do this by running this command:
```
echo 'export PATH="/usr/local/bin:$PATH"' >> $HOME/.bashrc
```
You may need to restart your shell for this to take effect, or refresh it with `source ~/.bashrc`.

If you want the global command then run:
```
cd tools/xdebug-toggle
ln -s `pwd`/xdebug-toggle /usr/local/bin/xdebug-toggle
```

## Make sure `xdebug-toggle` is executable

```
chmod +x /usr/local/bin/xdebug-toggle
```

## Usage
```
xdebug-toggle                            # outputs the current status
xdebug-toggle on                         # enables xdebug
xdebug-toggle off                        # disables xdebug
xdebug-toggle on|off --no-server-restart # toggles xdebug without restarting apache or php-fpm
```
[xdebug]: http://xdebug.org/
[xdebug-osx]: https://github.com/w00fz/xdebug-osx
[brew]: http://brew.sh/