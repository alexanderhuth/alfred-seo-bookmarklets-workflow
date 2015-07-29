# SEO Bookmarklets Workflow for Alfred
This [Alfred](http://www.alfredapp.com) workflow opens a website in browser-based SEO tools – much like your JavaScript-bookmarklets, but with less clicks.

## Installation
To install the workflow, download `seoBookmarklets.alfredworkflow` and double-click.

## How to Use It
Trigger the workflow with `seo`.

The workflow checks the frontmost application and if it’s a supported browser, the script opens the currently active URL in your SEO tools.

## Currently Supported SEO Tools/Bookmarklets
- [Sistrix](http://www.sistrix.com) Domain Overview: `http://de.sistrix.com/domain.tld`
- [Ahrefs](https://ahrefs.com/) Site Explorer Overview: `https://ahrefs.com/site-explorer/overview/subdomains?target=domain.tld`

### Adding More SEO Tools
You can expand this workflow by adding one new line per SEO tool: `open location toolURL & checkURL`.

You can "deactivate" specific SEO tools by commenting them out:
`-- open location toolURL & checkURL` or by deleting that specific line.

Define the “toolURL" variable at the top of the script: `property toolURL : "http://toolurlgoeshere"`

## Download
[SEO Bookmarklets Workflow for Alfred](#)

## Version History
### 1.0.0 – July 29, 2015
- Initial release
- Supports Safari, Google Chrome & Chromium
- Opens URL of currently active browser tab in Sistrix and Ahrefs
- Use `window.location.host` (JavaScript) to get host/domain name
- Don't open SEO tools for empty Safari tabs

### Roadmap
- Support more SEO tools/bookmarklets
- Easier enabling/adding and disabling of tools
- Warnings using Grunt/Notification Center
- Optional arguments to specifically trigger tools
- Support URLs in clipboard

## Credits
Icon made made by [Freepik](http://www.flaticon.com/authors/freepik)  from [www.flaticon.com](http://www.flaticon.com), licensed by [CC BY 3.0](http://creativecommons.org/licenses/by/3.0/).
Thanks to [Nathan Münnich](http://www.nathanmuennich.com) for the idea!