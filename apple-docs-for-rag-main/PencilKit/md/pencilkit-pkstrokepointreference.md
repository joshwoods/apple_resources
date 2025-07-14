

- PencilKit
-  PKStrokePointReference 

Class

# PKStrokePointReference

A class that represents the properties of a specific point along a stroke’s path.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
class PKStrokePointReference
```

## Topics

### Creating a stroke point object

init(location: CGPoint, timeOffset: TimeInterval, size: CGSize, opacity: CGFloat, force: CGFloat, azimuth: CGFloat, altitude: CGFloat)

Creates a new point with the provided properties.

init(location: CGPoint, timeOffset: TimeInterval, size: CGSize, opacity: CGFloat, force: CGFloat, azimuth: CGFloat, altitude: CGFloat, secondaryScale: CGFloat)

### Getting the point’s location

var location: CGPoint

The location of this point.

var timeOffset: TimeInterval

The time offset since the start of the stroke path in seconds.

### Getting the point’s touch data

var altitude: CGFloat

The altitude of this point in radians.

var azimuth: CGFloat

The azimuth of this point in radians.

var force: CGFloat

The amount of force applied by the touch.

### Getting the point’s drawing data

var size: CGSize

The size of the point.

var opacity: CGFloat

Opacity of the point.

var secondaryScale: CGFloat

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

