# Overview

This repo illustrates different ways that transpiled Elm can be used with Javascript Components. The priority was to keep the examples as simple as possible. There is no hot reloading or webpack conig.

Tested on OSX only for now.

## elm-embed

`elm-embed` demonstrates a simple embed of an html element.

## elm-port

`elm-port` demonstrates how to get the javascript code interoperate with the one transpiled from elm.

## elm-lib

`elm-lib` demonstrates how to use the transpiled code from elm as a library, whose functions can be called directly.


# Install

I use electron to rapidly develop javascript components on OSX, as an alternative to webpack dev-server and use `babel-register` for transpiling.

You must install electron-prebuilt globally:

    npm install -g electron-prebuilt

See the usage folders and double click on the `_electron.command` file in any usage folder.

  * elm-embed/usage/ -> _electron.command
  * elm-port/usage/ -> _electron.command

# Development

Install all elm package dependencies. In each elm folder:

    elm-embed/elm/ -> elm package install
    elm-port/elm/ -> elm package install

Double click the `_watch.command` file in any of the elm folder to automatically re-transpile elm whenever files change. Alternatively, call it from the command line `./_watch.command`.

Refresh the page in electron (command-R).
