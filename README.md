# SEO Bookmarklets Workflow for Alfred
This [Alfred](http://www.alfredapp.com) workflow opens a website URL in browser-based SEO tools – much like your JavaScript-bookmarklets, but with less clicks.

## Installation
To install the workflow, download `seoBookmarklets.alfredworkflow` and double-click.

## How to Use It
Trigger the workflow with `seo`. The workflow checks the frontmost application and if it’s a supported browser, the script opens the currently active URL in your SEO tools.

### Currently Supported SEO Tools/Bookmarklets
- [Sistrix](http://www.sistrix.com/) Domain Overview: `http://uk.sistrix.com/domain.tld`
- [Searchmetrics](http://www.searchmetrics.com/) SEO Research Overview: `http://suite.searchmetrics.com/en/research/domains/organic?url=domain.tld`
- [Ahrefs](https://ahrefs.com/) Site Explorer Overview: `https://ahrefs.com/site-explorer/overview/subdomains?target=domain.tld`

### Adding More SEO Tools
SEO tool URLs are listed in the `seoTools` variable at the top of the AppleScript in the workflow folder:  
`set seoTools to {"https://uk.sistrix.com/", "https://ahrefs.com/site-explorer/overview/subdomains?target=", "http://suite.searchmetrics.com/en/research/domains/organic?url="}`

You can easily add or remove URLs. You can also change URL parameters to specifically check one market or use a different language. Please make sure that the domain you're checking is always the final parameter.

### Turning off Notifications
You can turn off all notifications by removing or disconnecting the **Post Notification** object in the Alfred workflow window. If you only want to receive specific notifications, disable the unwanted ones by commenting them out in the AppleScript.

## Download
[SEO Bookmarklets Workflow for Alfred](https://github.com/alexanderhuth/alfred-seo-bookmarklets-workflow/raw/master/seoBookmarklets.alfredworkflow)

## Version History
### 1.5 – July 29, 2015
- Added Searchmetrics
- Easier enabling/adding and disabling of tools
	- List/group tool URLs as items of one variable
	- Use `repeat` to loop through SEO tools
- Notifications using Notification Center
- Don't open SEO tools for empty Chromium and Google Chrome tabs
- Code cleanup

### 1.0 – July 28, 2015
- Initial release
- Supports Safari, Google Chrome & Chromium
- Opens URL of currently active browser tab in Sistrix and Ahrefs
- Use `window.location.host` (JavaScript) to get host/domain name
- Don't open SEO tools for empty Safari tabs

### Roadmap
- Support more SEO tools/bookmarklets
- Optional arguments to specifically trigger tools
- Support URLs in clipboard

## Credits
[Icon](http://www.flaticon.com/free-icon/browser_14575) made made by [Freepik](http://www.flaticon.com/authors/freepik) from [www.flaticon.com](http://www.flaticon.com), licensed by [CC BY 3.0](http://creativecommons.org/licenses/by/3.0/).  
Thanks to [Nathan Münnich](http://www.nathanmuennich.com) for the idea!
