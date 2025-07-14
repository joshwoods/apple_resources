

- UIKit
- UIFindSession
-  allowsReplacementForCurrentlyHighlightedResult 

Instance Property

# allowsReplacementForCurrentlyHighlightedResult

A Boolean value that indicates whether to allow replacing the result the find panel is highlighting.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var allowsReplacementForCurrentlyHighlightedResult: Bool { get }
```

## Discussion

This property determines whether the find panel supports replacement for the currently highlighted item. If true, the system enables the Replace button in the find panel and the hardware keyboard shortcuts for replacement.

The default value is true if supportsReplacement is true.

## See Also

### Getting session information

var resultCount: Int

The total number of results the search matches.

var highlightedResultIndex: Int

The index of the result the find panel highlights.

var supportsReplacement: Bool

A Boolean value that indicates whether to allow replacing find panel results.

var searchResultDisplayStyle: UIFindSession.SearchResultDisplayStyle

The information the find panel includes in the summary of found results.

enum SearchResultDisplayStyle

Constants that describe the results summary the find panel UI includes.

