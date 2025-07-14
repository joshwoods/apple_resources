

- Model I/O
-  MDLAxisAlignedBoundingBox 

Structure

# MDLAxisAlignedBoundingBox

The minimal volume containing an object, used by the boundingBox(atTime:) method.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
struct MDLAxisAlignedBoundingBox
```

## Topics

### Initializers

init()

init(maxBounds: vector_float3, minBounds: vector_float3)

### Instance Properties

var maxBounds: vector_float3

The corner of the bounding box with the highest x-, y-, and z-coordinate values.

var minBounds: vector_float3

The corner of the bounding box with the lowest x-, y-, and z-coordinate values.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

