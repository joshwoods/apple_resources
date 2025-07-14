

- AppKit
- NSPasteboard
- NSPasteboard.PasteboardType
- NSPasteboard.PasteboardType.TextFinderOptionKey
-  textFinderCaseInsensitiveKey 

Type Property

# textFinderCaseInsensitiveKey

A Boolean value indicating whether the search is case insensitive.

macOS 10.7+

``` source
static let textFinderCaseInsensitiveKey: NSPasteboard.PasteboardType.TextFinderOptionKey
```

## Discussion

The value of this key must be an NSValue object containing a Boolean value. The value true indicates a case-insensitive search; false indicates a case-sensitive search.

## See Also

### Option Keys

static let textFinderMatchingTypeKey: NSPasteboard.PasteboardType.TextFinderOptionKey

A number object containing the match type to use.

