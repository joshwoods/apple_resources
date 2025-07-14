

- ARKit
-  ViewpointProperties 

Structure

# ViewpointProperties

The ViewpointProperties is a record of render camera transforms at some particular time.

visionOS 2.4+

``` source
struct ViewpointProperties
```

## Topics

### Instance Properties

var description: String

Textual representation of the viewpoint properties.

var deviceFromLeftViewpointTransform: simd_float4x4

The transformation matrix that converts from the left viewpoint to the device’s coordinate space.

var deviceFromRightViewpointTransform: simd_float4x4

The transformation matrix that converts from the left viewpoint to the device’s coordinate space.

## Relationships

### Conforms To

- CustomStringConvertible
- Sendable

