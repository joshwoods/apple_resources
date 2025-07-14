

- AppKit
- NSDocumentController
-  noteNewRecentDocumentURL(\_:) 

Instance Method

# noteNewRecentDocumentURL(\_:)

Adds or replaces an Open Recent menu item corresponding to the data located by the URL.

macOS

``` source
@MainActor
func noteNewRecentDocumentURL(_ url: URL)
```

## Parameters 

`url`  

The URL to evaluate.

## Discussion

`NSDocument` automatically calls this method when appropriate for `NSDocument`-based applications. Applications not based on `NSDocument` must also implement the application(_:openFile:) method in the application delegate to handle requests from the Open Recent menu command. You can override this method in an `NSDocument`-based application to prevent certain kinds of documents from getting into the list (but you have to identify them by URL).

## See Also

### Managing the Open Recent Menu

var maximumRecentDocumentCount: Int

The maximum number of items that may be presented in the standard Open Recent menu.

func clearRecentDocuments(Any?)

Empties the recent documents list for the application.

func noteNewRecentDocument(NSDocument)

Adds or replaces an Open Recent menu item corresponding to the document.

var recentDocumentURLs: [URL]

The list of recent-document URLs.

