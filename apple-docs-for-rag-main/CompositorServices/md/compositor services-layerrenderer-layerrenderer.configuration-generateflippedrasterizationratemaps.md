

- Compositor Services
- LayerRenderer
- LayerRenderer.Configuration
-  generateFlippedRasterizationRateMaps 

Instance Property

# generateFlippedRasterizationRateMaps

A Boolean value that indicates whether the layer renderer provides rasterization rate maps flipped around the y-axis.

visionOS 1.0+

``` source
var generateFlippedRasterizationRateMaps: Bool { get set }
```

## Discussion

When foveation is enabled and the value of this property is `true`, the layer renderer generates both flipped and nonflipped rasterization rate maps. When the value of this property is `false`, the layer renderer generates only the nonflipped rasterization rate maps. The default value of this property is `false`.

To generate flipped rasterization rate maps, the system must perform extra computational work during your app’s render loop. Enable this support only if your drawing engine requires these extra rate maps and you can afford the extra cost.

## See Also

### Configuring the foveation setting

var isFoveationEnabled: Bool

A value that indicates if the layer is using variable rasterization rates.

