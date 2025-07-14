

- UIKit
- UIFindSession
-  replaceAll(searchQuery:replacementString:options:) 

Instance Method

# replaceAll(searchQuery:replacementString:options:)

Replaces all matching instances of the query string with the replacement string you provide.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func replaceAll(
    searchQuery: String,
    replacementString: String,
    options: UITextSearchOptions?
)
```

## Parameters 

`searchQuery`  

The string to search for and replace, the user provides through the search text field of the system find panel.

`replacementString`  

The replacement string, the user provides through the replace text field of the system find panel.

`options`  

The object containing all the configurable options for the search.

## See Also

### Managing session interactions

func performSearch(query: String, options: UITextSearchOptions?)

Initiates a search for the query string you provide.

func performSingleReplacement(query: String, replacementString: String, options: UITextSearchOptions?)

Replaces a single instance of the query string with the replacement string you provide.

func highlightNextResult(in: UITextStorageDirection)

Updates the highlighted result to the next or previous match.

func invalidateFoundResults()

Invalidates the found ranges and updates the system find panel.

