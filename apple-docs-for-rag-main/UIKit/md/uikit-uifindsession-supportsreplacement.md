

- UIKit
- UIFindSession
-  supportsReplacement 

Instance Property

# supportsReplacement

A Boolean value that indicates whether to allow replacing find panel results.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var supportsReplacement: Bool { get }
```

## Discussion

This property determines whether the find panel shows the replacement UI.

The default value is false.

## See Also

### Getting session information

var resultCount: Int

The total number of results the search matches.

var highlightedResultIndex: Int

The index of the result the find panel highlights.

var allowsReplacementForCurrentlyHighlightedResult: Bool

A Boolean value that indicates whether to allow replacing the result the find panel is highlighting.

var searchResultDisplayStyle: UIFindSession.SearchResultDisplayStyle

The information the find panel includes in the summary of found results.

enum SearchResultDisplayStyle

Constants that describe the results summary the find panel UI includes.

