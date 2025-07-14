

- AppKit
- NSAnimation
-  NSAnimation.BlockingMode 

Enumeration

# NSAnimation.BlockingMode

These constants indicate the blocking mode of an `NSAnimation` object when it is running.

macOS

``` source
enum BlockingMode
```

## Overview

You specify one of these constants in the animationBlockingMode property.

## Topics

### Constants

case blocking

Requests the animation to run in the main thread in a custom run-loop mode that blocks user input.

case nonblocking

Requests the animation to run in a standard or specified run-loop mode that allows user input.

case nonblockingThreaded

Requests the animation to run in a separate thread that is spawned by the `NSAnimation` object.

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

enum Curve

These constants describe the curve of an animation—that is, the relative speed of an animation from start to finish.

typealias Progress

The animation progress, as a floating-point number between `0.0` and `1.0`.

NSAnimationProgressMark Notification Key

This constant is returned in the userInfo dictionary of the progressMarkNotification notification.

