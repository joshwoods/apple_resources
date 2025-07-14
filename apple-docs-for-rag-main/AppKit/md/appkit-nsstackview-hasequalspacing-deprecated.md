

- AppKit
- NSStackView
-  hasEqualSpacing Deprecated

Instance Property

# hasEqualSpacing

A Boolean value that indicates whether the spacing between adjacent views should be equal to each other.

macOS 10.9–10.11Deprecated

``` source
@MainActor
var hasEqualSpacing: Bool { get set }
```

Deprecated

Set distribution to NSStackView.Distribution.equalSpacing instead.

## Discussion

The distances between adjacent views in a stack view are either constrained to equal each other or settable to custom spacings using the setCustomSpacing(_:after:) method. The default value for the hasEqualSpacing property is false, which enables custom spacing. To require equal spacing, set this property to true, which disables the setCustomSpacing(_:after:) method.

With hasEqualSpacing set to false (the default), the Auto Layout constraints for spacing between views in a gravity area are as shown in the table of the spacing property.

If you specify equal spacing, the system changes these constraints to the values shown in the table below.

| Constraint | Value for constraint priority |
|----|----|
| inter-view spacing `==` the spacing property | hugging priority |
| inter-view spacing `≥` the spacing property | NSLayoutPriorityRequired |
| Equal inter-view spacing | NSLayoutPriorityDefaultLow |

Stack view hugging priority, identified as the constraint value in row 1, has the default value defaultLow. You can adjust hugging priority by using the setHuggingPriority(_:for:) method.

## See Also

### Related Documentation

func setHuggingPriority(NSLayoutConstraint.Priority, for: NSLayoutConstraint.Orientation)

Sets the Auto Layout priority for the stack view to minimize its size, for a specified user interface axis.

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

var distribution: NSStackView.Distribution

enum Distribution

