

- UIKit
-  UIViewAnimatingState 

Enumeration

# UIViewAnimatingState

Constants indicating the current state of the animation.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
enum UIViewAnimatingState
```

## Topics

### Constants

case inactive

The animations have not yet started executing. This is the initial state of the animator object.

case active

The animator object is active and animations are either running or paused. An animator moves to this state after the first call to startAnimation() or pauseAnimation(). It stays in the active state until the animations finish naturally or until you call the stopAnimation(_:) method.

case stopped

The animation is stopped. Putting an animation into this state ends the animation and leaves any animatable properties at their current values, instead of updating them to their intended final values. An animation cannot be started while in this state.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum UIViewAnimatingPosition

Constants indicating positions within the animation.

