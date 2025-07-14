

- Core Animation
-  CAMetalDisplayLink 

Class

# CAMetalDisplayLink

A class your Metal app uses to register for callbacks to synchronize its animations for a display.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class CAMetalDisplayLink
```

## Overview

CAMetalDisplayLink instances are a specialized way to interact with variable-rate displays when you need more control over the timing window to render your app’s frames. Controlling the timing window and rendering delay for frames can help you achieve smoother frame rates and avoid visual artifacts.

Tip

When working with less visually intensive apps or apps which don’t use Metal, use CADisplayLink to handle variable refresh rates.

Your app initializes a new Metal display link by providing a target CAMetalLayer. Set this instance’s delegate property to an implementation that encodes the rendering work for Metal to perform. With a set delegate, synchronize the display with a run loop to perform rendering on by calling the add(to:forMode:) method.

Once you associate the display link with a run loop, the system calls the delegate’s metalDisplayLink(_:needsUpdate:) method to request new frames. This method receives update requests based on the preferredFrameRateRange and preferredFrameLatency of the display link. The system makes a best effort to make callbacks at appropriate times. Your app should complete any commits to the Metal device’s MTLCommandQueue for rendering the display layer before calling present() on a drawable element.

Your app can disable notifications by setting isPaused to `true`. When your app finishes with a display link, call invalidate()to remove it from all run loops and the target.

## Topics

### Creating a Display Link

init(metalLayer: CAMetalLayer)

Creates a display link for Metal from a Core Animation layer.

### Configuring a Display Link

var preferredFrameRateRange: CAFrameRateRange

A range of frequencies your app allows for frame updates, affecting how often the system invokes your delegate’s callback.

var preferredFrameLatency: Float

The amount of time, in frames, your app requests to render a frame.

var delegate: (any CAMetalDisplayLinkDelegate)?

An instance of a type your app implements that responds to the system’s callbacks.

### Registering for Callbacks

func add(to: RunLoop, forMode: RunLoop.Mode)

Registers the display link with a run loop.

### Pausing Callbacks

var isPaused: Bool

A Boolean value that indicates whether the system suspends the display link’s notifications to the target.

### Deregistering for callbacks

func remove(from: RunLoop, forMode: RunLoop.Mode)

Removes a mode’s display link from a run loop.

func invalidate()

Removes the display link from all run loops for all modes.

### Classes

class Update

Stores information about a single update from a Metal display link instance.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Animation Timing

func CACurrentMediaTime() -> CFTimeInterval

Returns the current absolute time, in seconds.

class CAMediaTimingFunction

A function that defines the pacing of an animation as a timing curve.

protocol CAMediaTiming

Methods that model a hierarchical timing system, allowing objects to map time between their parent and local time.

class CADisplayLink

A timer object that allows your app to synchronize its drawing to the refresh rate of the display.

class Update

Stores information about a single update from a Metal display link instance.

protocol CAMetalDisplayLinkDelegate

A protocol your app implements to respond to callbacks from Core Animation for a Metal display link.

