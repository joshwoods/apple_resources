

- AppKit
- NSAnimation
-  NSAnimation.Curve 

Enumeration

# NSAnimation.Curve

These constants describe the curve of an animation—that is, the relative speed of an animation from start to finish.

macOS

``` source
enum Curve
```

## Overview

You initialize an `NSAnimation` object using one of these constants with init(duration:animationCurve:) and you can set it thereafter with the animationCurve property.

## Topics

### Constants

case easeInOut

Describes an S-curve in which the animation slowly speeds up and then slows down near the end of the animation. This constant is the default.

case easeIn

Describes an animation that slows down as it reaches the end.

case easeOut

Describes an animation that slowly speeds up from the start.

case linear

Describes an animation in which there is no change in frame rate.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum BlockingMode

These constants indicate the blocking mode of an `NSAnimation` object when it is running.

typealias Progress

The animation progress, as a floating-point number between `0.0` and `1.0`.

NSAnimationProgressMark Notification Key

This constant is returned in the userInfo dictionary of the progressMarkNotification notification.

