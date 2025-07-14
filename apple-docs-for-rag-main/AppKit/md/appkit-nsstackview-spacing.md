

- AppKit
- NSStackView
-  spacing 

Instance Property

# spacing

The minimum spacing, in points, between adjacent views in the stack view.

macOS 10.9+

``` source
@MainActor
var spacing: CGFloat { get set }
```

## Discussion

A stack view uses this property to define the minimum distance between views within a gravity area and between neighboring views in adjacent gravity areas. The default value for the spacing property is `8.0` points.

The automatically applied Auto Layout constraints for spacing are shown in the table below.

| Constraint | Value for constraint priority |
|----|----|
| inter-view spacing `==` the spacing property value | max (NSLayoutPriorityDefaultHigh, hugging priority) |
| inter-gravity-area spacing `==` the spacing property value | hugging priority |
| inter-view spacing `≥` the spacing property value | NSLayoutPriorityRequired |

The first row indicates that inter-view spacing is constrained to equal the value of the spacing property with a priority of at least defaultHigh; you can increase this by setting a higher stack view hugging priority with the setHuggingPriority(_:for:) method.

The second row indicates that the spacing between adjacent views in neighboring gravity areas is constrained to equal the value of the spacing property with the priority of the stack view’s hugging priority.

The third row indicates that inter-view spacing is allowed to grow larger than the value of the spacing property with a priority of NSLayoutPriorityRequired.

In combination, these constraints result in the following typical stack view behavior: In a stack view whose hasEqualSpacing property is set to false (the default) and whose hugging priority is left at defaultLow (the default), views within a gravity area remain a fixed distance from each other (equal to the value of the spacing property), and the distance between gravity areas grows and shrinks as the stack view grows and shrinks along its layout direction axis. If you set the hasEqualSpacing property to true and use the default hugging priority, then the distance between all adjacent views, including adjacent views in neighboring gravity areas, grows and shrinks as the stack view grows and shrinks.

## See Also

### Configuring the Stack View Layout

var orientation: NSUserInterfaceLayoutOrientation

The horizontal or vertical layout direction of the stack view.

enum NSUserInterfaceLayoutOrientation

The stack view layout directions, and user interface axes for hugging priority and clipping resistance.

var alignment: NSLayoutConstraint.Attribute

The view alignment within the stack view.

class let useDefaultSpacing: CGFloat

var edgeInsets: NSEdgeInsets

The geometric padding, in points, inside the stack view, surrounding its views.

var hasEqualSpacing: Bool

A Boolean value that indicates whether the spacing between adjacent views should be equal to each other.

Deprecated

var distribution: NSStackView.Distribution

enum Distribution

