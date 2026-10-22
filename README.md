# zwatch

Watches a Typst file for changes, recompiling it to WATCH_FILENAME and opens it
in zathura (which auto-reloads on change). Returns immediately; once zathura is
closed, the watcher is killed and WATCH_FILENAME is removed in the background.

## Usage

```
zwatch <file.typ>
```

## How to install with pm

You can use the Github installer from the ur:

```lua
ur.Github { user = "hugoocoto", repo = "zwatch", cmd = "" }
```

