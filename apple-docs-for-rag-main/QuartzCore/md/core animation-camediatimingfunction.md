

- Core Animation
-  CAMediaTimingFunction 

Class

# CAMediaTimingFunction

A function that defines the pacing of an animation as a timing curve.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class CAMediaTimingFunction
```

## Overview

`CAMediaTimingFunction` represents one segment of a function that defines the pacing of an animation as a timing curve. The function maps an input time normalized to the range `[0,1]` to an output time also in the range `[0,1]`.

You can create a media timing function by supplying your own cubic Bézier curve control points using the init(controlPoints:_:_:_:) method or by using one of the predefined timing functions.

## Topics

### Creating Timing Functions

convenience init(name: CAMediaTimingFunctionName)

Creates and returns a new instance of `CAMediaTimingFunction` configured with the predefined timing function specified by `name`.

init(controlPoints: Float, Float, Float, Float)

Returns an initialized timing function modeled as a cubic Bézier curve using the specified control points.

### Accessing the Control Points

func getControlPoint(at: Int, values: UnsafeMutablePointer&lt;Float>)

Returns the control point for the specified index.

### Constants

Predefined Timing Functions

Constants that specify system-provided timing functions, used by init(name:).

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Animation Timing

func CACurrentMediaTime() -> CFTimeInterval

Returns the current absolute time, in seconds.

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

