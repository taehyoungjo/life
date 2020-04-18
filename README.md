# Timeline

Simple timelines generated from Markdown.

Repurposed from Lim Chee Aun's [cheeaun.life](https://github.com/cheeaun/life)

Run `python -m http.server` in directory and navigate to `http://localhost:8000/`

## Features

- Events: List items in the format of `- DATE TEXT` where `-`, `DATE`, and `TEXT` are separated by a single space to render an event
- Dates: Dates of arbitrary specificity. See Datetime for range of formats
- Tags: Specified by `#` in `life.md` and `#life .event.tag-XXXX .time` and `#life .event.tag-XXX .time` in custom style sheet

### In progress

- Incorrect offsets with negative years
- `onmouseover` descriptions

## How to configure your _Timeline_

- `customStylesheetURL` - (_string_, default to `null`) Path to a custom stylesheet file, for those who doesn't like the default _theme_.
- `yearLength` - (_number_, default to `120`) The width of the year grids, in pixels.
- `hideAge` - (_boolean_, default to `false`) Option to hide age from year axis.

Added features

- `hideTags` - (_boolean_, default to `false`) Option to hide tags in event text

## Datetime

Modifications have been made from the original project in rendering dates. We now use `moment.js` instead of a custom parser. Years can be arbitrarily many digits and negative years render correctly.

### Supported formats

- `YYYY` with arbitrarily many digits
- `YYYY/MM`
- `YYYY/MM/DD`
- `YYYY/MM/DD:YYYY/MM/DD` or any combination of the above separated by a colon

## License

[MIT](http://cheeaun.mit-license.org/)
