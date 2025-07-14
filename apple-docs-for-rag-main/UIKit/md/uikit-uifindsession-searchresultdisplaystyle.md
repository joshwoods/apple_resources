

- UIKit
- UIFindSession
-  searchResultDisplayStyle 

Instance Property

# searchResultDisplayStyle

The information the find panel includes in the summary of found results.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var searchResultDisplayStyle: UIFindSession.SearchResultDisplayStyle { get set }
```

## See Also

### Getting session information

var resultCount: Int

The total number of results the search matches.

var highlightedResultIndex: Int

The index of the result the find panel highlights.

var supportsReplacement: Bool

A Boolean value that indicates whether to allow replacing find panel results.

var allowsReplacementForCurrentlyHighlightedResult: Bool

A Boolean value that indicates whether to allow replacing the result the find panel is highlighting.

enum SearchResultDisplayStyle

Constants that describe the results summary the find panel UI includes.

