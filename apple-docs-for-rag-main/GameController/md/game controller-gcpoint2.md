

- Game Controller
-  GCPoint2 

Structure

# GCPoint2

A structure that represents a normalized point in a two-dimensional coordinate system.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.3+tvOS 17.4+visionOS 1.1+

``` source
struct GCPoint2
```

## Topics

### Creating a point

init()

Creates a two dimensional point with coordinates `(0, 0)`.

init(x: Float, y: Float)

Creates a two dimensional point with the given coordinates.

func GCPoint2Make(Float, Float) -> GCPoint2

Returns a point with the specified coordinates in a two-dimensional coordinate system.

let GCPoint2Zero: GCPoint2

The origin for a two dimensional point.

### Accessing coordinates

var x: Float

The x-coordinate for the point.

var y: Float

The y-coordinate for the point.

### Comparing and converting points

func GCPoint2Equal(GCPoint2, GCPoint2) -> Bool

Returns whether two points are equal.

func NSStringFromGCPoint2(GCPoint2) -> String

Returns a string representation of a point.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Getting the value

var value: GCPoint2

The axis input represented as a normalized point in a two-dimensional coordinate system.

**Required**

var valueDidChangeHandler: ((any GCPhysicalInputElement, any GCAxis2DInput, GCPoint2) -> Void)?

The block that the axis element calls when its value changes.

**Required**

var lastValueTimestamp: TimeInterval

The time of the most recent value change.

**Required**

var lastValueLatency: TimeInterval

The time in seconds between the last value change and the current time.

**Required**

