

- Metal
- MTLAccelerationStructureInstanceDescriptor
-  mask 

Instance Property

# mask

A mask to use for the instance when testing a ray against the geometry.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var mask: UInt32
```

## Discussion

Metal reserves the top 24 bits for future use.

## See Also

### Customizing Intersection and Hit Tests for the Instance

var intersectionFunctionTableOffset: UInt32

An offset for determining which function in the intersection function table Metal needs to call when testing a ray against the instance.

var options: MTLAccelerationStructureInstanceOptions

The options for the instance.

