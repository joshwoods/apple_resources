

- AppKit
- NSStackView
-  detachesHiddenViews 

Instance Property

# detachesHiddenViews

A Boolean value that indicates whether the stack view removes hidden views from its view hierarchy.

macOS 10.11+

``` source
@MainActor
var detachesHiddenViews: Bool { get set }
```

## Discussion

When the value of this property is true, setting the isHidden property of a view to true causes the stack view to remove hidden views from its view hierarchy and put them in the detachedViews property. Changing the view’s isHidden property to false causes the stack view to add the view back to the view hierarchy. When the value of this property is false, views remain in the view hierarchy, even when they are hidden. The default value of this property is true.

## See Also

### Configuring Dynamic Behavior for a Stack View

func setClippingResistancePriority(NSLayoutConstraint.Priority, for: NSLayoutConstraint.Orientation)

Sets the Auto Layout priority for resisting clipping of views in the stack view when Auto Layout attempts to reduce the stack view’s size.

func setHuggingPriority(NSLayoutConstraint.Priority, for: NSLayoutConstraint.Orientation)

Sets the Auto Layout priority for the stack view to minimize its size, for a specified user interface axis.

