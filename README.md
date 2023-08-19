# j2e Alfred workflow

## Alfred workflow to convert between JSON and EDN

This is fast-n-dirty [Alfred](https://www.alfredapp.com/) workflow that transforms JSON files to EDN format or vice versa. The conversion is local, so you may not be afraid of your client's data leaks.

This may be useful for some paranoid Clojure developers.

## Installation

**j2e** workflow depends on [borkdude](https://github.com/borkdude)'s great utility called [jet](https://github.com/borkdude/jet). You have to install if before using this workflow.

* Install **brew**: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

* Install **jet**: `brew install borkdude/brew/jet`

## Demo

![j2e demo](img/e2j.gif)

## Usage

* Copy your JSON data into the clipboard (usually with `CMD+C`)

* Start Alfred prompt and enter `j2e`. Press `ENTER`. Now your EDN data should replace your JSON data in the clipboard.

* Click in any text editor or form where you need your EDN and press `CMD+V`.

(if you need to convert EDN to JSON, do exactly same, except the Alfred keyword will become `e2j`.

## Known problems

1. Invalid data will be silently ignored, not converted. 

## What are those formats?

* https://www.json.org/json-en.html

* https://github.com/edn-format/edn
