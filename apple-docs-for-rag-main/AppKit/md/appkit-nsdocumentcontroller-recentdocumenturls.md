

- AppKit
- NSDocumentController
-  recentDocumentURLs 

Instance Property

# recentDocumentURLs

The list of recent-document URLs.

macOS

``` source
@MainActor
var recentDocumentURLs: [URL] { get }
```

## Discussion

This property contains an array of NSURL objects corresponding to the recently opened documents. Do not override this property.

## See Also

### Managing the Open Recent Menu

var maximumRecentDocumentCount: Int

The maximum number of items that may be presented in the standard Open Recent menu.

func clearRecentDocuments(Any?)

Empties the recent documents list for the application.

func noteNewRecentDocumentURL(URL)

Adds or replaces an Open Recent menu item corresponding to the data located by the URL.

func noteNewRecentDocument(NSDocument)

Adds or replaces an Open Recent menu item corresponding to the document.

