

- Core Animation
- CATiledLayer
-  levelsOfDetailBias 

Instance Property

# levelsOfDetailBias

The number of magnified levels of detail for this layer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var levelsOfDetailBias: Int { get set }
```

## Discussion

Defaults to 0. Each previous level of detail is twice the resolution of the later. For example, specifying a value of 2 means that the layer has two extra levels of detail: 2x and 4x.

## See Also

### Levels of detail

var levelsOfDetail: Int

The number of levels of detail maintained by this layer.

