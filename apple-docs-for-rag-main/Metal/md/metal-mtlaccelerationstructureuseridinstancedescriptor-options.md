

- Metal
- MTLAccelerationStructureUserIDInstanceDescriptor
-  options 

Instance Property

# options

The options for the instance.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var options: MTLAccelerationStructureInstanceOptions
```

## See Also

### Customizing Intersection and Hit Tests for the Instance

var intersectionFunctionTableOffset: UInt32

An offset for determining which function in the intersection function table Metal calls when testing a ray against the instance.

var mask: UInt32

A mask to use for the instance when testing a ray against the geometry.

