

- Core Animation
- CATiledLayer
-  levelsOfDetail 

Instance Property

# levelsOfDetail

The number of levels of detail maintained by this layer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var levelsOfDetail: Int { get set }
```

## Discussion

Defaults to 1. Each level of detail is half the resolution of the previous level. If too many levels are specified for the current size of the layer, then the number of levels is clamped to the maximum value (the bottom most level of detail must contain at least a single pixel in each dimension.)

## See Also

### Levels of detail

var levelsOfDetailBias: Int

The number of magnified levels of detail for this layer.

