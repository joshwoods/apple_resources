

- AppKit
- NSPasteboard
- NSPasteboard.PasteboardType
-  NSPasteboard.PasteboardType.FindPanelSearchOptionKey 

Structure

# NSPasteboard.PasteboardType.FindPanelSearchOptionKey

Search options for the find panel.

macOS

``` source
struct FindPanelSearchOptionKey
```

## Topics

### Search Option Keys

static let findPanelCaseInsensitiveSearch: NSPasteboard.PasteboardType.FindPanelSearchOptionKey

A Boolean value indicating whether the search is case-insensitive.

static let findPanelSubstringMatch: NSPasteboard.PasteboardType.FindPanelSearchOptionKey

A number object containing the match type to use in the find panel.

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

struct TextFinderOptionKey

Search options for text in Finder.

