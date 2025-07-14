

- AppKit
- NSStackView
-  orientation 

Instance Property

# orientation

The horizontal or vertical layout direction of the stack view.

macOS 10.9+

``` source
@MainActor
var orientation: NSUserInterfaceLayoutOrientation { get set }
```

## Discussion

Default value is NSUserInterfaceLayoutOrientation.horizontal. For values that apply to this property, see NSUserInterfaceLayoutOrientation.

## See Also

### Configuring the Stack View Layout

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

enum Distribution

