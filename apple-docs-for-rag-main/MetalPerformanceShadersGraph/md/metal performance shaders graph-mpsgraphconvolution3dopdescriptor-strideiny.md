

- Metal Performance Shaders Graph
- MPSGraphConvolution3DOpDescriptor
-  strideInY 

Instance Property

# strideInY

The scale that maps`y`-coordinate of destination to `y`-coordinate of source.

iOS 16.3+iPadOS 16.3+Mac Catalyst 16.3+macOS 13.2+tvOS 16.3+visionOS 1.0+

``` source
var strideInY: Int { get set }
```

## Discussion

Source `y`-coordinate, `sy` is computed from destination `y`-coordinate, `dy` as `sy = strideInY*dy`. Default value is 1.

