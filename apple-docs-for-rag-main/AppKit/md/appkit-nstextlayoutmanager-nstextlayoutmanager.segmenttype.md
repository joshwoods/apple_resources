

- AppKit
- NSTextLayoutManager
-  NSTextLayoutManager.SegmentType 

Enumeration

# NSTextLayoutManager.SegmentType

Values that describe the rendering of selection boundaries.

macOS 12.0+

``` source
enum SegmentType
```

## Topics

### Kinds of text selection segments

case highlight

The segment behavior suitable for highlighting.

case selection

The segment behavior suitable for selection rendering.

case standard

The standard segment, matching the typographic bounds of the range.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Causing layout generation

var textViewportLayoutController: NSTextViewportLayoutController

Returns text viewport layout controller associated with the layout manager’s text container.

func invalidateLayout(for: NSTextRange)

Invalidates the layout information for specified text range.

func textLayoutFragment(for: any NSTextLocation) -> NSTextLayoutFragment?

Returns the text layout fragment from the document at the specified location.

func textLayoutFragment(for: CGPoint) -> NSTextLayoutFragment?

Returns the text layout fragment at the position you specify in the text container.

func ensureLayout(for: CGRect)

Performs the layout for filling the bounds you specify inside the last text container.

func ensureLayout(for: NSTextRange)

Performs the layout for specified text range.

func enumerateTextLayoutFragments(from: (any NSTextLocation)?, options: NSTextLayoutFragment.EnumerationOptions, using: (NSTextLayoutFragment) -> Bool) -> (any NSTextLocation)?

Enumerates the text layout fragments starting at the specified location.

struct SegmentOptions

Values that describe where and how the framework extends segments of a selection.

