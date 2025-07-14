

- UIKit
- UIFindSession
-  highlightNextResult(in:) 

Instance Method

# highlightNextResult(in:)

Updates the highlighted result to the next or previous match.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func highlightNextResult(in direction: UITextStorageDirection)
```

## Parameters 

`direction`  

The direction, either forward or backward, to move through the search results.

## Discussion

The system calls this method when a person taps the next or previous button, or enters `Return` or `Shift+Return` on a hardware keyboard while the search field has focus.

## See Also

### Managing session interactions

func performSearch(query: String, options: UITextSearchOptions?)

Initiates a search for the query string you provide.

func performSingleReplacement(query: String, replacementString: String, options: UITextSearchOptions?)

Replaces a single instance of the query string with the replacement string you provide.

func replaceAll(searchQuery: String, replacementString: String, options: UITextSearchOptions?)

Replaces all matching instances of the query string with the replacement string you provide.

func invalidateFoundResults()

Invalidates the found ranges and updates the system find panel.

