

- UIKit
- UIFindSession
-  performSearch(query:options:) 

Instance Method

# performSearch(query:options:)

Initiates a search for the query string you provide.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func performSearch(
    query: String,
    options: UITextSearchOptions?
)
```

## Parameters 

`query`  

The string to search, the user provides through the search text field of the system find panel.

`options`  

The object containing all the configurable options for the search.

## Discussion

The system calls this method when the user initiates a search for a string in your app’s text content.

## See Also

### Managing session interactions

func performSingleReplacement(query: String, replacementString: String, options: UITextSearchOptions?)

Replaces a single instance of the query string with the replacement string you provide.

func replaceAll(searchQuery: String, replacementString: String, options: UITextSearchOptions?)

Replaces all matching instances of the query string with the replacement string you provide.

func highlightNextResult(in: UITextStorageDirection)

Updates the highlighted result to the next or previous match.

func invalidateFoundResults()

Invalidates the found ranges and updates the system find panel.

