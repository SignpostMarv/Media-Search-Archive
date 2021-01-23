# Media Search Archive

Static site generator for
	[twitch-clip-notes](https://github.com/SignpostMarv/twitch-clip-notes)
	data.

# See Also

* [Satisfactory Q&A Clips Archive](https://archive.satisfactory.video/) - Serves as an archive for Q&A Clips for Coffee Stain Studio's Satisfactory-related livestream

# Changelog

## 2021-01-23
* Updated build to reflect support for additional clip sources
* Implemented dark mode
* Dropped relevance search in favour of chronological
* Added site description to page footer

## 2021-01-22
* Updated build to reflect changes in topic metadata
* Corrected typo in changelog
* Updated build to refactor headings & navigation
* Corrected typo in navigation link
* Updated build to rely less on hardcoded legacy twitch clips, favouring partially dynamic injection
* Moved site to a new domain
* Amended 404 page
* Amended generated page titles for the FAQ

## 2021-01-21
* Added Icons
* Refactored search page to be built by eleventy for template reuse
* Corrected dates in changelog
* Updated github repo links
* Switched from what would've been an ever-expanding monolithic JSON-LD file
	to [modular data defined in a separate repo](
		https://github.com/Satisfactory-Clips-Archive/Media-Archive-Metadata
	)
* Updated portions of site build to use consistently sorted topic metadata
* Finally got around to updating the search tool's topics url prefix

## 20201-01-20
* Updated site build with latest livestream data
* Tweaked template output

## 20201-01-18
* Adjusted opengraph data

## 20201-01-17
* Implemented additional structured data & other metadata.

## 20201-01-16
* Implemented ability to specify structured data not sourced from markdown front matter.
* Moved search page to avoid inclusion of html extension.

## 20201-01-14
* Implemented more structured data.

## 20201-01-13
* Fixed bugs.

* Implemented a change to the client-side search index,
	where the data was split by date to aid in browser caching.

	Splitting by date means not having to discard the previous search index when a new livestream comes out.

	There's a slightly longer load delay on first visit as each index & set of documents are fetched, but subsequent visits and date-filtered searches should load faster.
