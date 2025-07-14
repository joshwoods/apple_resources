

- UIKit
- UIFindSession
-  invalidateFoundResults() 

Instance Method

# invalidateFoundResults()

Invalidates the found ranges and updates the system find panel.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func invalidateFoundResults()
```

## Discussion

If the searchText for the find interaction is non-empty, a call to this method this triggers a call to performSearch(query:options:) immediately after to begin a new search.

## See Also

### Managing session interactions

func performSearch(query: String, options: UITextSearchOptions?)

Initiates a search for the query string you provide.

func performSingleReplacement(query: String, replacementString: String, options: UITextSearchOptions?)

Replaces a single instance of the query string with the replacement string you provide.

func replaceAll(searchQuery: String, replacementString: String, options: UITextSearchOptions?)

Replaces all matching instances of the query string with the replacement string you provide.

func highlightNextResult(in: UITextStorageDirection)

Updates the highlighted result to the next or previous match.

