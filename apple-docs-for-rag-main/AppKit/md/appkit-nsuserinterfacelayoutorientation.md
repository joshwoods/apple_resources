

- AppKit
-  NSUserInterfaceLayoutOrientation 

Enumeration

# NSUserInterfaceLayoutOrientation

The stack view layout directions, and user interface axes for hugging priority and clipping resistance.

macOS 10.9+

``` source
enum NSUserInterfaceLayoutOrientation
```

## Topics

### Constants

case horizontal

The horizontal orientation.

case vertical

The vertical orientation.

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

### Configuring the Stack View Layout

var orientation: NSUserInterfaceLayoutOrientation

The horizontal or vertical layout direction of the stack view.

var alignment: NSLayoutConstraint.Attribute

The view alignment within the stack view.

var spacing: CGFloat

The minimum spacing, in points, between adjacent views in the stack view.

class let useDefaultSpacing: CGFloat

var edgeInsets: NSEdgeInsets

The geometric padding, in points, inside the stack view, surrounding its views.

var hasEqualSpacing: Bool

A Boolean value that indicates whether the spacing between adjacent views should be equal to each other.

Deprecated

var distribution: NSStackView.Distribution

enum Distribution

