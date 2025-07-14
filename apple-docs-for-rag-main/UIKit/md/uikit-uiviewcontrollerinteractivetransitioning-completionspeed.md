

- UIKit
- UIViewControllerInteractiveTransitioning
-  completionSpeed 

Instance Property

# completionSpeed

Called when the system needs the speed at which to complete an interactive transition, after the interactive portion is finished.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional var completionSpeed: CGFloat { get }
```

## Return Value

Default value is `1.0`, which corresponds to the total (noninteractive) transition duration scaled by the percentage of the transition remaining. Value must be greater than `0.0`.

## See Also

### Providing a transition’s completion characteristics

var completionCurve: UIView.AnimationCurve

Called when the system needs the animation completion curve for an interactive view controller transition.

