

- Metal
- MTLAccelerationStructureInstanceDescriptor
-  intersectionFunctionTableOffset 

Instance Property

# intersectionFunctionTableOffset

An offset for determining which function in the intersection function table Metal needs to call when testing a ray against the instance.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var intersectionFunctionTableOffset: UInt32
```

## Discussion

By default, after Metal finds an intersection between a ray and a primitive, it runs your specified intersection function to determine whether the ray actually hit the primitive. To determine which function in the intersection table to call, Metal adds this property to the value in the instance’s intersectionFunctionTableOffset, and looks up the entry at that index.

## See Also

### Customizing Intersection and Hit Tests for the Instance

var options: MTLAccelerationStructureInstanceOptions

The options for the instance.

var mask: UInt32

A mask to use for the instance when testing a ray against the geometry.

