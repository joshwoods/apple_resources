

- Core Animation
-  CADisplayLink 

Class

# CADisplayLink

A timer object that allows your app to synchronize its drawing to the refresh rate of the display.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+macOS 14.0+tvOS 9.0+visionOS 1.0+

``` source
class CADisplayLink
```

## Mentioned in 

Optimizing ProMotion refresh rates for iPhone 13 Pro and iPad Pro

## Overview

Your app initializes a new display link by providing a target object and a selector to call when the system updates the screen. To synchronize your display loop with the display, your application adds it to a run loop using the add(to:forMode:) method.

Once you associate the display link with a run loop, the system calls the selector on the target when the screen’s contents need to update. The target can read the display link’s timestamp property to retrieve the time the system displayed the previous frame. For example, an app that displays movies might use `timestamp` to calculate which video frame to display next. An app that performs its own animations might use `timestamp` to determine where and how visible objects appear in the upcoming frame.

The duration property provides the amount of time between frames at the maximumFramesPerSecond. To calculate the actual frame duration, use targetTimestamp - timestamp. You can use this value in your app to calculate the frame rate of the display, the approximate time the system displays the next frame, and to adjust the drawing behavior so that the next frame is ready in time to display.

Your app can disable notifications by setting isPaused to `true`. Also, if your app can’t provide frames in the time the system provides, you may want to choose a slower frame rate. An app with a slower but consistent frame rate appears smoother to the user than an app that skips frames. You can define the number of frames per second by setting preferredFramesPerSecond.

When your app finishes with a display link, call invalidate() to remove it from all run loops and to disassociate it from the target.

The code listing below shows how to create a display link and add it to the current run loop. The display link invokes the step function, which prints the target timestamp with each screen update.

- Swift
- Objective-C

```
func createDisplayLink() {
    let displaylink = CADisplayLink(target: self,
                                    selector: #selector(step))

    displaylink.add(to: .current,
                    forMode: .defaultRunLoopMode)
}

func step(displaylink: CADisplayLink) {
    print(displaylink.targetTimestamp)
}
```

```
- (void)createDisplayLink {
    CADisplayLink *displayLink = [CADisplayLink displayLinkWithTarget:self
                                                             selector:@selector(step:)];
    [displayLink addToRunLoop:[NSRunLoop currentRunLoop]
                      forMode:NSRunLoopCommonModes];
}

- (void)step:(CADisplayLink *)sender {
    NSLog(@"%f", sender.targetTimestamp);
}
```

You shouldn’t subclass CADisplayLink.

### Preferred and Actual Frame Rates

You control a display link’s frame rate (the number of times the system calls the selector of its target, per second) by setting preferredFramesPerSecond. However, the actual frames per second may differ from the preferred value you set; actual frame rates are always a factor of the maximum refresh rate of the device. For example, if your device’s maximum refresh rate is 60 frames per second (defined by maximumFramesPerSecond), actual frame rates include 15, 20, 30, and 60 frames per second. If you set a display link’s preferred frame rate to a value higher than the maximum, the actual frame rate is the maximum.

In iOS 15, frame rate availability can change due to the system factoring in the system policy and user preference — including Low Power Mode, critical thermal state, and accessibility settings.

The system rounds, to the nearest factor, preferred frame rates that aren’t a divisor of the maximum frame rate. For example, setting a preferred frame rate to either 26 or 35 frames per second on a device with a maximum refresh rate of 60 frames per second yields an actual frame rate of 30 times per second.

The code listing below shows how to calculate the actual frame rate by dividing 1 by your display link’s timestamp subtracted from its targetTimestamp.

- Swift
- Objective-C

```
// Calculate the actual frame rate.
let actualFramesPerSecond = 1 / (displaylink.targetTimestamp - displaylink.timestamp)
```

```
// Calculate the actual frame rate.
double actualFramesPerSecond = 1 / (displaylink.targetTimestamp - displaylink.timestamp);
```

Note

If your app needs more control over refresh rate to ensure smooth rendering of frames, use CAMetalDisplayLink and the information from CAMetalLayer instances to render frames.

## Topics

### Creating a Display Link

init(target: Any, selector: Selector)

Creates a display link for a target that calls its selector.

### Configuring a Display Link

var duration: CFTimeInterval

The time interval between screen refresh updates.

var preferredFrameRateRange: CAFrameRateRange

A range of frequencies your app allows for frame updates, affecting how often the system invokes your delegate’s callback.

var preferredFramesPerSecond: Int

A frequency your app prefers for frame updates, affecting how often the system invokes your delegate’s callback.

Deprecated

var isPaused: Bool

A Boolean value that indicates whether the system suspends the display link’s notifications to the target.

var timestamp: CFTimeInterval

The time interval that represents when the last frame displayed.

var targetTimestamp: CFTimeInterval

The time interval that represents when the next frame displays.

var frameInterval: Int

The number of frames that must pass before the display link notifies the target again.

Deprecated

### Scheduling a Display Link to Send Notifications

func add(to: RunLoop, forMode: RunLoop.Mode)

Registers the display link with a run loop.

func remove(from: RunLoop, forMode: RunLoop.Mode)

Removes the display link from the run loop for the given mode.

func invalidate()

Removes the display link from all run loop modes.

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

### Related Documentation

Presenting content on a connected display

Fill connected displays with additional content from your app.

### Animation Timing

func CACurrentMediaTime() -> CFTimeInterval

Returns the current absolute time, in seconds.

class CAMediaTimingFunction

A function that defines the pacing of an animation as a timing curve.

protocol CAMediaTiming

Methods that model a hierarchical timing system, allowing objects to map time between their parent and local time.

class CAMetalDisplayLink

A class your Metal app uses to register for callbacks to synchronize its animations for a display.

class Update

Stores information about a single update from a Metal display link instance.

protocol CAMetalDisplayLinkDelegate

A protocol your app implements to respond to callbacks from Core Animation for a Metal display link.

