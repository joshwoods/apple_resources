

- UIKit
- UIViewControllerInteractiveTransitioning
-  completionCurve 

Instance Property

# completionCurve

Called when the system needs the animation completion curve for an interactive view controller transition.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional var completionCurve: UIView.AnimationCurve { get }
```

## Return Value

Default value is UIView.AnimationCurve.easeInOut, with other possible values described in the UIView.AnimationCurve type definition.

## See Also

### Providing a transition’s completion characteristics

var completionSpeed: CGFloat

Called when the system needs the speed at which to complete an interactive transition, after the interactive portion is finished.

