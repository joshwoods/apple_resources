

- AppKit
- NSPasteboard
- NSPasteboard.PasteboardType
- NSPasteboard.PasteboardType.TextFinderOptionKey
-  textFinderMatchingTypeKey 

Type Property

# textFinderMatchingTypeKey

A number object containing the match type to use.

macOS 10.7+

``` source
static let textFinderMatchingTypeKey: NSPasteboard.PasteboardType.TextFinderOptionKey
```

## Discussion

The value of this key must be an NSNumber containing an NSTextFinder.MatchingType value that indicates the type of search matching to perform.

## See Also

### Option Keys

static let textFinderCaseInsensitiveKey: NSPasteboard.PasteboardType.TextFinderOptionKey

A Boolean value indicating whether the search is case insensitive.

