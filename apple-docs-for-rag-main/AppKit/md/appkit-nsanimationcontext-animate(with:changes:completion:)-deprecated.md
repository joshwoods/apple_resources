

- AppKit
- NSAnimationContext
-  animate(with:changes:completion:) Deprecated

Type Method

# animate(with:changes:completion:)

Animates changes to one or more views using the specified SwiftUI animation.

macOS 15.0–15.0Deprecated

``` source
static func animate(
    with animation: Animation,
    changes: () -> Void,
    completion: (() -> Void)? = nil
)
```

Deprecated

Use animate(_:changes:completion:) instead.

## Parameters 

`animation`  

The animation to use for the changes.

`changes`  

A closure that contains the changes to animate.

`completion`  

A closure to execute after the animation completes.

## Discussion

Use this method to leverage SwiftUI animations from AppKit code, creating a more consistent animation experience if your app incorporates code from both frameworks.

For more information, read Unifying your app’s animations.

Note

When a SwiftUI animation is used for animating AppKit’s NSAnimatablePropertyContainer, the animations are run in-process, and are not backed by CAAnimations in the render server.

