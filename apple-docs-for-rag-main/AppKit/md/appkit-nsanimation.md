

- AppKit
-  NSAnimation 

Class

# NSAnimation

An object that manages the timing and progress of animations in the user interface.

macOS

``` source
class NSAnimation
```

## Overview

NSAnimation also lets you link together multiple animations so that when one animation ends another one starts. It does not provide any drawing support for animation and does not directly deal with views, targets, or actions.

Note

For simple tasks requiring a timing mechanism, consider using Timer.

NSAnimation objects have several characteristics, including duration, frame rate, and animation curve, which describes the relative speed of the animation over its course. You can set progress marks in an animation, each of which specifies a percentage of the animation completed; when an animation reaches a progress mark, it notifies its delegate and posts a notification to any observers. Animations execute in one of three blocking modes: blocking, non-blocking on the main thread, and non-blocking on a separate thread. The non-blocking modes permit the handling of user events while the animation is running.

### Subclassing Notes

The usual usage pattern for `NSAnimation` is to make a subclass that overrides (at least) the currentProgress property to invoke the superclass implementation and then perform whatever animation action is needed. The method implementation might use the currentValue property and then use that value to update some drawing; as a consequence of getting the current value, the method animation(_:valueForProgress:) is sent to the delegate (if there is a delegate that implements the method). For more information on subclassing `NSAnimation`, see Animation Programming Guide for Cocoa.

## Topics

### Initializing an NSAnimation Object

init(duration: TimeInterval, animationCurve: NSAnimation.Curve)

Returns an `NSAnimation` object initialized with the specified duration and animation-curve values.

### Configuring an Animation

var animationBlockingMode: NSAnimation.BlockingMode

The blocking mode of the animation.

var runLoopModesForAnimating: [RunLoop.Mode]?

An array of strings representing the run loop modes in which the animation can run.

var animationCurve: NSAnimation.Curve

The timing curve for the animation.

var duration: TimeInterval

The duration of the animation, in seconds.

var frameRate: Float

The number of frame updates per second to generate for the animation.

### Managing the Delegate

var delegate: (any NSAnimationDelegate)?

The animation delegate.

### Controlling and Monitoring an Animation

func start()

Starts the animation represented by the receiver.

func stop()

Stops the animation represented by the receiver.

var isAnimating: Bool

A Boolean value indicating whether the animation is in progress.

var currentProgress: NSAnimation.Progress

The current progress of the animation.

var currentValue: Float

The current value of the animation effect, based on the current progress

### Managing Progress Marks

func addProgressMark(NSAnimation.Progress)

Adds the progress mark to the receiver.

func removeProgressMark(NSAnimation.Progress)

Removes progress mark from the receiver.

var progressMarks: [NSNumber]

An array of floating-point numbers representing current progress marks.

### Linking Animations Together

func start(when: NSAnimation, reachesProgress: NSAnimation.Progress)

Starts running the animation represented by the receiver when another animation reaches a specific progress mark.

func stop(when: NSAnimation, reachesProgress: NSAnimation.Progress)

Stops running the animation represented by the receiver when another animation reaches a specific progress mark.

func clearStart()

Clears linkage to another animation that causes the receiver to start.

func clearStop()

Clears linkage to another animation that causes the receiver to stop.

### Constants

enum Curve

These constants describe the curve of an animation—that is, the relative speed of an animation from start to finish.

enum BlockingMode

These constants indicate the blocking mode of an `NSAnimation` object when it is running.

typealias Progress

The animation progress, as a floating-point number between `0.0` and `1.0`.

NSAnimationProgressMark Notification Key

This constant is returned in the userInfo dictionary of the progressMarkNotification notification.

### Notifications

class let progressMarkNotification: NSNotification.Name

Posted when the current progress of a running animation reaches one of its progress marks.

### Initializers

init?(coder: NSCoder)

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSViewAnimation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Custom Animations

protocol NSAnimationDelegate

A set of optional methods implemented by delegates of NSAnimation objects.

