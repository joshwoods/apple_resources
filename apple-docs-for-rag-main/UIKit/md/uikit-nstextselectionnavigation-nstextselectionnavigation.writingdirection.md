

- UIKit
- NSTextSelectionNavigation
-  NSTextSelectionNavigation.WritingDirection 

Enumeration

# NSTextSelectionNavigation.WritingDirection

Values that describe the writing direction inside a text selection.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
enum WritingDirection
```

## Topics

### Writing directions

case leftToRight

The value that defines the left to right writing direction.

case rightToLeft

The value that defines the right to left writing direction.

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

### Changing the characteristics of the selection

func baseWritingDirection(at: any NSTextLocation) -> NSTextSelectionNavigation.WritingDirection

Returns the base writing direction at the location you specify.

**Required**

func textLayoutOrientation(at: any NSTextLocation) -> NSTextSelectionNavigation.LayoutOrientation

Returns the layout orientation at the location you specify.

enum LayoutOrientation

Values that describe the possible layout orientations.

