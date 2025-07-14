

- Core Image
- CIFilter
- Generator Filters
- CILenticularHaloGenerator
-  haloOverlap 

Instance Property

# haloOverlap

The separation of colors in the halo.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var haloOverlap: Float { get set }
```

**Required**

## Discussion

A value of `0` means the halo colors don't overlap. A value of `1` means the halo colors fully overlap, creating a white halo.

