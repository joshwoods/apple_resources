

- Game Controller
-  GCAcceleration 

Structure

# GCAcceleration

A three-dimensional acceleration vector.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
struct GCAcceleration
```

## Topics

### Getting Acceleration Values

var x: Double

The acceleration measurement along the x-axis, in multiples of earth’s gravity.

var y: Double

The acceleration measurement along the y-axis, in multiples of earth’s gravity.

var z: Double

The acceleration measurement along the z-axis, in multiples of earth’s gravity.

### Initializers

init()

Creates an acceleration structure.

init(x: Double, y: Double, z: Double)

Creates an acceleration structure with the specified values.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Accessing Gravity and Acceleration Data

var acceleration: GCAcceleration

The total acceleration of the controller that includes gravity and the acceleration the user applies to the controller.

var gravity: GCAcceleration

The gravity acceleration vector from the controller’s reference frame.

var userAcceleration: GCAcceleration

The acceleration that the user applies to the controller.

