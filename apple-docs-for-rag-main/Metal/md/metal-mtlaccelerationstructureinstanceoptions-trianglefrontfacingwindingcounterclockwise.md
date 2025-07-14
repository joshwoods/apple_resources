

- Metal
- MTLAccelerationStructureInstanceOptions
-  triangleFrontFacingWindingCounterClockwise 

Type Property

# triangleFrontFacingWindingCounterClockwise

Specifies that the instance specifies front facing triangles in counter-clockwise order.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
static var triangleFrontFacingWindingCounterClockwise: MTLAccelerationStructureInstanceOptions { get }
```

## See Also

### Usage Options

static var disableTriangleCulling: MTLAccelerationStructureInstanceOptions

An option that turns off culling for this instance if ray intersector has culling enabled.

static var opaque: MTLAccelerationStructureInstanceOptions

Specifies that intersectors should treat the instance as opaque.

static var nonOpaque: MTLAccelerationStructureInstanceOptions

Specifies that intersectors should treat the instance as non-opaque.

