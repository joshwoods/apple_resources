

- Core Animation
- CAMetalDisplayLink
-  CAMetalDisplayLink.Update 

Class

# CAMetalDisplayLink.Update

Stores information about a single update from a Metal display link instance.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class Update
```

## Topics

### Timing the Next Animation Frame

var targetPresentationTimestamp: CFTimeInterval

The time the system estimates until the display of the next frame.

var targetPresentationTimestamp: CFTimeInterval

The time the system estimates until the display of the next frame.

### Drawing the Next Frame

var targetTimestamp: CFTimeInterval

A deadline that indicates when your app needs to finish rendering to the drawable.

var drawable: any CAMetalDrawable

The Metal drawable your app uses to render the next frame.

var targetTimestamp: CFTimeInterval

A deadline that indicates when your app needs to finish rendering to the drawable.

var drawable: any CAMetalDrawable

The Metal drawable your app uses to render the next frame.

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

class CAMetalDisplayLink

A class your Metal app uses to register for callbacks to synchronize its animations for a display.

protocol CAMetalDisplayLinkDelegate

A protocol your app implements to respond to callbacks from Core Animation for a Metal display link.

