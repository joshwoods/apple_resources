

- Metal
- MTLLibraryOptimizationLevel
-  MTLLibraryOptimizationLevel.size 

Case

# MTLLibraryOptimizationLevel.size

An optimization option for the Metal compiler that prioritizes minimizing the size of its output binaries, which may also reduce compile time.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
case size
```

## Mentioned in 

Minimizing the Binary Size of a Shader Library

## Discussion

This option is similar to MTLLibraryOptimizationLevel.default, but adds optimizations that prioritize minimizing a shader’s executable size, which may also reduce compile time.

## See Also

### Optimization Options

case `default`

An optimization option for the Metal compiler that prioritizes runtime performance.

