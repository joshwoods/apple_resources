

- Metal Performance Shaders Graph
- MPSGraphConvolution2DOpDescriptor
-  strideInY 

Instance Property

# strideInY

The scale that maps `y`-coordinate of the destination to `y`-coordinate of the source.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var strideInY: Int { get set }
```

## Discussion

Source `y`-coordinate, `sy` is computed from destination `y`-coordinate, `dy` as `sy = strideInY*dy`. Default value is 1.

