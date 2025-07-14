

- AppKit
- NSStackView
-  edgeInsets 

Instance Property

# edgeInsets

The geometric padding, in points, inside the stack view, surrounding its views.

macOS 10.9+

``` source
@MainActor
var edgeInsets: NSEdgeInsets { get set }
```

## Discussion

The default value is `(0, 0, 0, 0)`. Edge insets remain as they are if you change the value of a stack view’s orientation property or the value of its inherited userInterfaceLayoutDirection property.

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

var hasEqualSpacing: Bool

A Boolean value that indicates whether the spacing between adjacent views should be equal to each other.

Deprecated

var distribution: NSStackView.Distribution

enum Distribution

