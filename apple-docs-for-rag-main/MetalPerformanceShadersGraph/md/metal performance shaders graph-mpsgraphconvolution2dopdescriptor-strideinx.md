

- Metal Performance Shaders Graph
- MPSGraphConvolution2DOpDescriptor
-  strideInX 

Instance Property

# strideInX

The scale that maps `x`-coordinate of the destination to `x`-coordinate of the source.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var strideInX: Int { get set }
```

## Discussion

Source `x`-coordinate, `sx` is computed from destination `x`-coordinate, `dx` as `sx = strideInX*dx`. Default value is 1.

