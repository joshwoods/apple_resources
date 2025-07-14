

- UIKit
- UIViewImplicitlyAnimating
-  addAnimations(\_:) 

Instance Method

# addAnimations(\_:)

Adds the specified animation block to the animator.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional func addAnimations(_ animation: @escaping () -> Void)
```

## Parameters 

`animation`  

A block containing the animations to add to the animator object. This block has no return value and takes no parameters.

## Discussion

Use this method to add new animation blocks to your custom animator object. The animations in the specified block should run alongside any previously configured animations, starting at the current time and finishing at the same time as any original animations. Your implementation must be able to handle multiple calls to this method.

## See Also

### Modifying animations

func addAnimations(() -> Void, delayFactor: CGFloat)

Adds the specified animation block to the animator with a delay.

func addCompletion((UIViewAnimatingPosition) -> Void)

Adds the specified completion block to the animator.

func continueAnimation(withTimingParameters: (any UITimingCurveProvider)?, durationFactor: CGFloat)

Adjusts the final timing and duration of a paused animation.

