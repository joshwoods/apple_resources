

- Metal
- MTLAccelerationStructureInstanceOptions
-  opaque 

Type Property

# opaque

Specifies that intersectors should treat the instance as opaque.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
static var opaque: MTLAccelerationStructureInstanceOptions { get }
```

## See Also

### Usage Options

static var disableTriangleCulling: MTLAccelerationStructureInstanceOptions

An option that turns off culling for this instance if ray intersector has culling enabled.

static var triangleFrontFacingWindingCounterClockwise: MTLAccelerationStructureInstanceOptions

Specifies that the instance specifies front facing triangles in counter-clockwise order.

static var nonOpaque: MTLAccelerationStructureInstanceOptions

Specifies that intersectors should treat the instance as non-opaque.

