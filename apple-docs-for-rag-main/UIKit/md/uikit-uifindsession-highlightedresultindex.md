

- UIKit
- UIFindSession
-  highlightedResultIndex 

Instance Property

# highlightedResultIndex

The index of the result the find panel highlights.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var highlightedResultIndex: Int { get }
```

## Discussion

To indicate no highlighted result, return `nil` (Swift) or NSNotFound (Objective-C).

## See Also

### Getting session information

var resultCount: Int

The total number of results the search matches.

var supportsReplacement: Bool

A Boolean value that indicates whether to allow replacing find panel results.

var allowsReplacementForCurrentlyHighlightedResult: Bool

A Boolean value that indicates whether to allow replacing the result the find panel is highlighting.

var searchResultDisplayStyle: UIFindSession.SearchResultDisplayStyle

The information the find panel includes in the summary of found results.

enum SearchResultDisplayStyle

Constants that describe the results summary the find panel UI includes.

