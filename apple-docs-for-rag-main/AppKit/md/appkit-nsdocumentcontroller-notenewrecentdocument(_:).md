

- AppKit
- NSDocumentController
-  noteNewRecentDocument(\_:) 

Instance Method

# noteNewRecentDocument(\_:)

Adds or replaces an Open Recent menu item corresponding to the document.

macOS

``` source
@MainActor
func noteNewRecentDocument(_ document: NSDocument)
```

## Parameters 

`document`  

The document to evaluate.

## Discussion

This method constructs a URL and calls noteNewRecentDocumentURL(_:). Subclasses might override this method to prevent certain documents or kinds of documents from getting into the list.

## See Also

### Managing the Open Recent Menu

var maximumRecentDocumentCount: Int

The maximum number of items that may be presented in the standard Open Recent menu.

func clearRecentDocuments(Any?)

Empties the recent documents list for the application.

func noteNewRecentDocumentURL(URL)

Adds or replaces an Open Recent menu item corresponding to the data located by the URL.

var recentDocumentURLs: [URL]

The list of recent-document URLs.

