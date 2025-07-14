

- AppKit
- NSAnimation
-  NSAnimation.Progress 

Type Alias

# NSAnimation.Progress

The animation progress, as a floating-point number between `0.0` and `1.0`.

macOS

``` source
typealias Progress = Float
```

## Discussion

An animation progress value is returned in the `userInfo` dictionary of an progressMarkNotification notification.

## See Also

### View-Based Animations

class NSViewAnimation

An animation of an app’s views, limited to changes in frame location and size, and to fade-in and fade-out effects.

protocol NSAnimatablePropertyContainer

A set of methods that defines a way to add animation to an existing class with a minimum of API impact.

class NSAnimationContext

An animation context, which contains information about environment and state.

enum NSAnimationEffect

The type for standard system animation effects, which include both display and sound.

Deprecated

