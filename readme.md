# Dumbsweeper

A tiny (746 bytes as of the last update), simple, and feature-less (hence "dumb", it has only the bare essentials) Minesweeper game packed into a data URL, made for [Shrink](https://shrink.hackclub.com).

Copy and paste this into your browser's address bar to try it:

```
data:text/html, "test" <> {} '' 
```

## gourlgolfing (Go URL Golfing)

A tool I built to help create Dumbsweeper.

It's essentially a wrapper around existing utilities to make code golfing data URL websites easier.

To use it, install Go and run:

```bash
go install github.com/reztheperson/dumbsweeper/gourlgolfing@latest
```

- `gourlgolfing dev <folder>`: Combines `style.css`, `index.html`, and `script.js` into a single file and serves it at `localhost:8080`.
* `gourlgolfing build <folder>`: Combines `style.css`, `index.html`, and `script.js` into one file, minifies it by stripping unnecessary whitespace and comments, converts it to a data URL, and saves the output to `uri.txt`.
