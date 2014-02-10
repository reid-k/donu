changelog
=========

2014-02-10:

* Added configuration option `LOG`, which causes donu to keep timestamped records of URIs and the programs they were given to.
    * Defaults to `False`.
    * Logs are stored in `~/.config/donu/logs/` as `YYYY-MM-DD.log`

2014-02-03:

* **IMPORTANT**: moved config file from `~/.donu.conf` to `~/.config/donu/donu.conf`
* Added configuration option `EDITOR`, which unsurprisingly specifies an editor to use
    * Defaults to vim.
* Implemented option to open config file in specified editor
    * Changes made will not take effect until the next time donu is run
* Implemented option to open current URI in specified editor
    * Once done, opens new instance of donu with resulting edit
    * Using this requires donu to have write access to `~/.config/donu/`, where it creates a file named `donu-tmp-<donu's current pid>` to pass to the editor.
* Changed from [clint](https://pypi.python.org/pypi/clint/) to [colorama](https://pypi.python.org/pypi/colorama) for color support
* Made the menu numbers look nicer and show more color, if enabled
* Comments added for legibility, as requested
* Added short usage message in response to too many arguments as well as too few
* Added long help message in response to `-h` and `--help`
