

- UIKit
- UISnapBehavior
-  snapPoint 

Instance Property

# snapPoint

The point to which to snap.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var snapPoint: CGPoint { get set }
```

## Discussion

The initial value of this property is the value you passed in to the init(item:snapTo:) method. Changing this value updates the dynamic item and potentially puts it in motion again.

The coordinate system of the point depends on how you initialized the underlying dynamic animator, as described in the overview of UIDynamicAnimator.

## See Also

### Configuring a snap behavior

var damping: CGFloat

The amount of oscillation of a dynamic item during the conclusion of a snap.

