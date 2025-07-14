

- UIKit
- UIPageControl
-  UIPageControl.Direction 

Enumeration

# UIPageControl.Direction

Decribes the layout direction of a page control’s indicators.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
enum Direction
```

## Topics

### Directions

case natural

A direction that infers the lay out from the system’s locale.

case leftToRight

A direction that lays out the page indicators from left to right.

case rightToLeft

A direction that lays out the page indicators from right to left.

case topToBottom

A direction that lays out the page indicators from top to bottom.

case bottomToTop

A direction that lays out the page indicators from bottom to top.

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

### Customizing the layout direction

var direction: UIPageControl.Direction

The layout direction of the page indicators.

