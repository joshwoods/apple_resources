

- Quick Look UI
-  QLPreviewViewStyle 

Enumeration

# QLPreviewViewStyle

Styles for a Preview View.

macOS 10.7+

``` source
enum QLPreviewViewStyle
```

## Topics

### Choosing a Preview Style

case normal

Provides the default preview style for larger, full-sized previews.

case compact

Provides a compact preview style suited for smaller previews or inspectors.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a Preview View

init!(frame: NSRect, style: QLPreviewViewStyle)

Creates a preview view with the provided frame and style.

init!(frame: NSRect)

Creates a preview view with the provided frame.

