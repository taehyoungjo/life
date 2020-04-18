# Timeline

Simple timelines generated from Markdown.

I've repurposed Lim Chee Aun's [cheeaun.life](https://github.com/cheeaun/life) to act as a tool for creating general purpose timelines.

## Features

### In progress

## How to setup your own _Life_

## How to configure your _Life_

1. Make a copy of `config.example.json`, rename it to `config.json`.
2. Only commit it in `gh-pages` branch.

The configuration:

- `customStylesheetURL` - (_string_, default to `null`) Path to a custom stylesheet file, for those who doesn't like the default _theme_.
- `yearLength` - (_number_, default to `120`) The width of the year grids, in pixels.
- `hideAge` - (_boolean_, default to `false`) Option to hide age from year axis.

Added features

- `hideTags` - (_boolean_, default to `false`) Option to hide tags in event text

## Datetime

Modifications have been made from the original project in rendering dates. We now use moment.js instead of a custom parser. Years can be arbitrary many digits and negative years are also supported.

### Supported formats

- YYYY/MM/DD
- YYYY/MM/DD:YYYY/MM/DD

## Other people's Lives

Here's [a compilation of Lives from the people who have forked Life](https://github.com/cheeaun/life/wiki/Lives).

## License

[MIT](http://cheeaun.mit-license.org/)
