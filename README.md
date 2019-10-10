This repository covers the following recipe from code.activestate.com:

[LOG WATCHER (TAIL -F *.LOG) 
](https://code.activestate.com/recipes/577968/)

*Created by Giampaolo Rodolà on Tue, 29 Nov 2011*

A python class which "watches" a directory and calls a callback(filename, lines) function every time one of the files being watched gets written, in real time.

Practically speaking, this can be compared to "tail -F *.log" UNIX command, but instead of having lines printed to stdout a python function gets called.

Similarly to tail, it takes care of "watching" new files which are created after initialization and "unwatching" those ones which are removed in the meantime. This means you'll be able to "follow" and support also rotating log files.

## Usage

If you already have the [State Tool] installed you can simply run

```
state activate ActiveState-Recipes/recipe-577968-log-watcher-tail-f-log
```

If you do not have the [State Tool] installed you can use the following convenient one-liner.

Linux: 
```
sh <(curl -q https://platform.activestate.com/dl/cli/install.sh) && state activate ActiveState-Recipes/recipe-577968-log-watcher-tail-f-log
```

Windows: 
```
powershell "IEX(New-Object Net.WebClient).downloadString('https://platform.activestate.com/dl/cli/install.ps1')" && state activate ActiveState-Recipes/recipe-577968-log-watcher-tail-f-log
```

macOS: not yet supported

[State Tool]: https://www.activestate.com/products/platform/state-tool/

### Advanced Usage

See [original recipe](https://code.activestate.com/recipes/577968/) for advanced usage information