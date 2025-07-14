

- UIKit
- NSTextLayoutFragment
-  NSTextLayoutFragment.State 

Enumeration

# NSTextLayoutFragment.State

Values that describe the possible layout states.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
enum State
```

## Topics

### Constants that describe layout bounds

case calculatedUsageBounds

The layout fragment measurements are available without text line fragments.

case estimatedUsageBounds

The text layout manager hasn’t performed a full layout yet for the region covered by this layout fragment and is returning an estimated bounds.

case layoutAvailable

Measurements for the text line fragments and layout fragment are available.

case none

No layout information is available.

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

### Getting element information

var state: NSTextLayoutFragment.State

The layout information state.

var rangeInElement: NSTextRange

The range inside the text element relative to the document origin.

var textElement: NSTextElement?

The parent text element.

