

- AppKit
- NSStackView
-  alignment 

Instance Property

# alignment

The view alignment within the stack view.

macOS 10.9+

``` source
@MainActor
var alignment: NSLayoutConstraint.Attribute { get set }
```

## Discussion

The default value for this property depends on whether the stack view is horizontal or vertical:

- *Horizontal*: The default value is NSLayoutConstraint.Attribute.centerY.

- *Vertical*: The default value is NSLayoutConstraint.Attribute.centerX.

These constants are described as part of the NSLayoutConstraint.Attribute enumeration in NSLayoutConstraint; see that enumeration for the other possible alignment values.

Note

Using certain values in this property can result in unexpected behavior:

- Specifying the NSLayoutConstraint.Attribute.notAnAttribute constant can result in an ambiguous layout.

- A value inappropriate for the layout direction is ignored; for example, the system ignores a value of NSLayoutConstraint.Attribute.centerX for the horizontal layout.

## See Also

### Configuring the Stack View Layout

var orientation: NSUserInterfaceLayoutOrientation

The horizontal or vertical layout direction of the stack view.

enum NSUserInterfaceLayoutOrientation

The stack view layout directions, and user interface axes for hugging priority and clipping resistance.

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

