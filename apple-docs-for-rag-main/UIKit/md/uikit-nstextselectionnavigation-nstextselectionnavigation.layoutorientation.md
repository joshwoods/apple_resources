

- UIKit
- NSTextSelectionNavigation
-  NSTextSelectionNavigation.LayoutOrientation 

Enumeration

# NSTextSelectionNavigation.LayoutOrientation

Values that describe the possible layout orientations.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
enum LayoutOrientation
```

## Topics

### Layout orientations

case horizontal

The value that defines horizontal layout orientation.

case vertical

The value that defines vertical layout orientation.

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

enum WritingDirection

Values that describe the writing direction inside a text selection.

func textLayoutOrientation(at: any NSTextLocation) -> NSTextSelectionNavigation.LayoutOrientation

Returns the layout orientation at the location you specify.

