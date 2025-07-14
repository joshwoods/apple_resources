

- AppKit
- NSAnimationContext
-  animate(\_:changes:completion:) 

Type Method

# animate(\_:changes:completion:)

Animate changes to one or more views using the specified SwiftUI animation.

macOS 15.0+

``` source
static func animate(
    _ animation: Animation,
    changes: () -> Void,
    completion: (() -> Void)? = nil
)
```

## Parameters 

`animation`  

The animation to use for the changes.

`changes`  

A closure containing the changes to animate.

`completion`  

A closure to execute after the animation completes.

## Discussion

Animations performed using this method can be smoothly retargeted while preserving velocity, just like animations in SwiftUI views.

```
// Grow the window with a smooth spring animation
NSAnimationContext.animate(.smooth) {
    var scaledFrame = myWindowContentView.frame.applying(CGAffineTransform(scaleX: 1.5, y: 1.5)
    myWindowContentView.setFrameSize(myScaledFrame)
}
```

Note

When a SwiftUI animation is used for animating AppKit’s `NSAnimatablePropertyContainer`s, the animations are run in-process, and are not backed by `CAAnimation`s in the render server.

