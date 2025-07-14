

- Metal
- MTLAccelerationStructureGeometryDescriptor
-  intersectionFunctionTableOffset 

Instance Property

# intersectionFunctionTableOffset

An index into the intersection table for determining which intersection function Metal calls when it intersects a ray with the acceleration structure.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var intersectionFunctionTableOffset: Int { get set }
```

## See Also

### Specifying Base Geometry Properties

var label: String?

A label for the geometry structure, suitable for debugging.

var opaque: Bool

A Boolean value that determines whether the geometry data in the acceleration structure needs to skip triangle-intersection tests.

var allowDuplicateIntersectionFunctionInvocation: Bool

A Boolean value that indicates whether Metal calls the ray-intersection test more than once per primitive on the structure.

