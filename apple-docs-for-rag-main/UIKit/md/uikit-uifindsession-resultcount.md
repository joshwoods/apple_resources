

- UIKit
- UIFindSession
-  resultCount 

Instance Property

# resultCount

The total number of results the search matches.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var resultCount: Int { get }
```

## See Also

### Getting session information

var highlightedResultIndex: Int

The index of the result the find panel highlights.

var supportsReplacement: Bool

A Boolean value that indicates whether to allow replacing find panel results.

var allowsReplacementForCurrentlyHighlightedResult: Bool

A Boolean value that indicates whether to allow replacing the result the find panel is highlighting.

var searchResultDisplayStyle: UIFindSession.SearchResultDisplayStyle

The information the find panel includes in the summary of found results.

enum SearchResultDisplayStyle

Constants that describe the results summary the find panel UI includes.

