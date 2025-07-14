

- Core Animation
-  CACurrentMediaTime() 

Function

# CACurrentMediaTime()

Returns the current absolute time, in seconds.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+

``` source
func CACurrentMediaTime() -> CFTimeInterval
```

## Return Value

A `CFTimeInterval` derived by calling `mach_absolute_time()` and converting the result to seconds.

## Mentioned in 

Optimizing ProMotion refresh rates for iPhone 13 Pro and iPad Pro

## See Also

### Animation Timing

class CAMediaTimingFunction

A function that defines the pacing of an animation as a timing curve.

protocol CAMediaTiming

Methods that model a hierarchical timing system, allowing objects to map time between their parent and local time.

class CADisplayLink

A timer object that allows your app to synchronize its drawing to the refresh rate of the display.

class CAMetalDisplayLink

A class your Metal app uses to register for callbacks to synchronize its animations for a display.

class Update

Stores information about a single update from a Metal display link instance.

protocol CAMetalDisplayLinkDelegate

A protocol your app implements to respond to callbacks from Core Animation for a Metal display link.

