

- Metal
- MTLAccelerationStructureUsage
-  preferFastBuild 

Type Property

# preferFastBuild

An option that specifies that Metal needs to build the acceleration structure quickly, even if that reduces ray-tracing performance.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
static var preferFastBuild: MTLAccelerationStructureUsage { get }
```

## Discussion

Typically, you specify this option for acceleration structures that you need to create or refit inside performance-sensitive code.

## See Also

### Usage Options

static var refit: MTLAccelerationStructureUsage

An option that specifies that you can refit the acceleration structure if the geometry changes.

static var extendedLimits: MTLAccelerationStructureUsage

A structure usage option that indicates you intend to use larger ray-tracing limits for the acceleration structure.

