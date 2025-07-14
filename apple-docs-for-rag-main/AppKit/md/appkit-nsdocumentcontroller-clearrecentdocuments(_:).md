

- AppKit
- NSDocumentController
-  clearRecentDocuments(\_:) 

Instance Method

# clearRecentDocuments(\_:)

Empties the recent documents list for the application.

macOS

``` source
@IBAction @MainActor
func clearRecentDocuments(_ sender: Any?)
```

## Discussion

This is the action for the Clear menu command, but it can be called directly if necessary.

## See Also

### Managing the Open Recent Menu

var maximumRecentDocumentCount: Int

The maximum number of items that may be presented in the standard Open Recent menu.

func noteNewRecentDocumentURL(URL)

Adds or replaces an Open Recent menu item corresponding to the data located by the URL.

func noteNewRecentDocument(NSDocument)

Adds or replaces an Open Recent menu item corresponding to the document.

var recentDocumentURLs: [URL]

The list of recent-document URLs.

