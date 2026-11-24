# zwatch

Watches a Typst file for changes, recompiling it to a PDF in a fresh per-run
directory (`/tmp/zwatch.XXXXXX/<name>.pdf`) and opens it in zathura (which
auto-reloads on change). Returns immediately; once zathura is closed, the
watcher is killed and the directory is removed in the background. You can run
several zwatch instances at the same time, even on the same file.

## Usage

```
zwatch <file.typ>
```

## How to install with pm

You can use the Github installer from the ur:

```lua
ur.Github { user = "hugoocoto", repo = "zwatch", cmd = ":" }
```

## Download

You can grab the file directly too:

```sh
curl -fsSLO https://raw.githubusercontent.com/hugoocoto/zwatch/refs/heads/main/zwatch
```
