

- AppKit
- NSStackView
-  NSStackView.Distribution 

Enumeration

# NSStackView.Distribution

macOS 10.11+

``` source
enum Distribution
```

## Topics

### Constants

case equalCentering

case equalSpacing

case fill

case fillEqually

case fillProportionally

case gravityAreas

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

enum NSUserInterfaceLayoutOrientation

The stack view layout directions, and user interface axes for hugging priority and clipping resistance.

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

