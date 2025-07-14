

- Metal Performance Shaders Graph
- MPSGraphConvolution3DOpDescriptor
-  strideInX 

Instance Property

# strideInX

The scale that maps`x`-coordinate of destination to `x`-coordinate of source.

iOS 16.3+iPadOS 16.3+Mac Catalyst 16.3+macOS 13.2+tvOS 16.3+visionOS 1.0+

``` source
var strideInX: Int { get set }
```

## Discussion

Source `x`-coordinate, `sx` is computed from destination `x`-coordinate, `dx` as `sx = strideInX*dx`. Default value is 1.

