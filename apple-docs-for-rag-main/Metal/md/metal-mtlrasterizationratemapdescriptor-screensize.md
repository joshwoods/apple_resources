

- Metal
- MTLRasterizationRateMapDescriptor
-  screenSize 

Instance Property

# screenSize

The size of the viewport coordinate system, in logical pixels.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
var screenSize: MTLSize { get set }
```

## Mentioned in 

Creating a Rasterization Rate Map

## Discussion

Metal ignores the depth component of this property.

The viewport coordinate system’s origin is always at `(0,0)` and this property determines its size.

