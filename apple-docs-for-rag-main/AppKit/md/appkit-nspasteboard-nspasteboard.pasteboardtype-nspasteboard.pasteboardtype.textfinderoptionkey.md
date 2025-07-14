

- AppKit
- NSPasteboard
- NSPasteboard.PasteboardType
-  NSPasteboard.PasteboardType.TextFinderOptionKey 

Structure

# NSPasteboard.PasteboardType.TextFinderOptionKey

Search options for text in Finder.

macOS

``` source
struct TextFinderOptionKey
```

## Topics

### Option Keys

static let textFinderCaseInsensitiveKey: NSPasteboard.PasteboardType.TextFinderOptionKey

A Boolean value indicating whether the search is case insensitive.

static let textFinderMatchingTypeKey: NSPasteboard.PasteboardType.TextFinderOptionKey

A number object containing the match type to use.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Option Keys

struct FindPanelSearchOptionKey

Search options for the find panel.

