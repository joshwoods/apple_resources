

- Core Animation
-  CAMediaTiming 

Protocol

# CAMediaTiming

Methods that model a hierarchical timing system, allowing objects to map time between their parent and local time.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
protocol CAMediaTiming
```

## Overview

Absolute time is defined as mach time converted to seconds. The CACurrentMediaTime() function is provided as a convenience for getting the current absolute time.

The conversion from parent time to local time has two stages:

1.  Conversion to “active local time.” This includes the point at which the object appears in the parent object’s timeline and how fast it plays relative to the parent.

2.  Conversion from “active local time” to “basic local time.” The timing model allows for objects to repeat their basic duration multiple times and, optionally, to play backwards before repeating.

## Topics

### Animation Start Time

var beginTime: CFTimeInterval

Specifies the begin time of the receiver in relation to its parent object, if applicable.

**Required**

var timeOffset: CFTimeInterval

Specifies an additional time offset in active local time.

**Required**

### Repeating Animations

var repeatCount: Float

Determines the number of times the animation will repeat.

**Required**

var repeatDuration: CFTimeInterval

Determines how many seconds the animation will repeat for.

**Required**

### Duration and Speed

var duration: CFTimeInterval

Specifies the basic duration of the animation, in seconds.

**Required**

var speed: Float

Specifies how time is mapped to receiver’s time space from the parent time space.

**Required**

### Playback Modes

var autoreverses: Bool

Determines if the receiver plays in the reverse upon completion.

**Required**

var fillMode: CAMediaTimingFillMode

Determines if the receiver’s presentation is frozen or removed once its active duration has completed.

**Required**

### Constants

Fill Modes

These constants determine how the timed object behaves once its active duration has completed. They are used with the fillMode property.

## Relationships

### Conforming Types

- CAAnimation
- CAAnimationGroup
- CABasicAnimation
- CAEAGLLayer
- CAEmitterCell
- CAEmitterLayer
- CAGradientLayer
- CAKeyframeAnimation
- CALayer
- CAMetalLayer
- CAOpenGLLayer
- CAPropertyAnimation
- CAReplicatorLayer
- CAScrollLayer
- CAShapeLayer
- CASpringAnimation
- CATextLayer
- CATiledLayer
- CATransformLayer
- CATransition

## See Also

### Animation Timing

func CACurrentMediaTime() -> CFTimeInterval

Returns the current absolute time, in seconds.

class CAMediaTimingFunction

A function that defines the pacing of an animation as a timing curve.

class CADisplayLink

A timer object that allows your app to synchronize its drawing to the refresh rate of the display.

class CAMetalDisplayLink

A class your Metal app uses to register for callbacks to synchronize its animations for a display.

class Update

Stores information about a single update from a Metal display link instance.

protocol CAMetalDisplayLinkDelegate

A protocol your app implements to respond to callbacks from Core Animation for a Metal display link.

