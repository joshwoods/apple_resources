

- MapKit
- MKLocalSearchCompletion
-  subtitleHighlightRanges 

Instance Property

# subtitleHighlightRanges

The ranges of characters to highlight in the subtitle string.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.11.4+tvOS 9.2+visionOS 1.0+

``` source
var subtitleHighlightRanges: [NSValue] { get }
```

## Discussion

This property contains an array of NSValue objects, each of which contains an NSRange type defining a range of characters in the subtitle string. Use this property to identify the ranges of characters in the subtitle string that you want to highlight. Highlighting the matching text of a search completion is optional, but it’s a best practice for providing helpful information to the user.

## See Also

### Getting the search completions

var title: String

The title string associated with the point of interest.

var subtitle: String

The subtitle (if any) associated with the point of interest.

var titleHighlightRanges: [NSValue]

The ranges of characters to highlight in the title string.

