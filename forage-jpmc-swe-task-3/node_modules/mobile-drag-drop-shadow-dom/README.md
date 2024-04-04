

# Polyfill for HTML 5 drag'n'drop _with Shadow DOM support_

[![npmversion](https://img.shields.io/npm/v/mobile-drag-drop-shadow-dom.svg)](https://www.npmjs.com/package/mobile-drag-drop-shadow-dom)

> :warning: ** This is a fork ** Forked from the excellent [`timruffles/mobile-drag-drop`](https://github.com/timruffles/mobile-drag-drop),
> which unfortunately does not work with within Shadow DOM.  This repository
> preserves only the compiled output of the original (Typescript) library, incorporating insights
> from [a GitHub Issue re: Shadow DOM support](https://github.com/timruffles/mobile-drag-drop/issues/115)
> to add Shadow DOM support.  It also calls `polyfill()` directly, removing
> the public API in favor of an opinionative side-effect.  Tested in Chrome, iOS
> and OSX Safari.
>
> Below acknowledgements preserved from the original [`README.md`](https://github.com/timruffles/mobile-drag-drop)

## Thanks

To the [amazing contributors](https://github.com/timruffles/mobile-drag-drop/graphs/contributors) who've provided massive extensions and fixes to the original.

<a href="http://twitter.com/rem">@rem</a> - who created the original demo used to demo this shim's drop-in nature.


## License

[MIT License](LICENSE)
