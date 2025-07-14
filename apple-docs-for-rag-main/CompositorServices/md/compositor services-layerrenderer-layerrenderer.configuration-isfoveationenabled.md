

- Compositor Services
- LayerRenderer
- LayerRenderer.Configuration
-  isFoveationEnabled 

Instance Property

# isFoveationEnabled

A value that indicates if the layer is using variable rasterization rates.

visionOS 1.0+

``` source
var isFoveationEnabled: Bool { get set }
```

## Discussion

Foveation support lets you reduce the amount of high-resolution drawing you do. With foveation, the system renders content someone looks at directly using a higher resolution than content in the person’s peripheral vision. This behavior lets you render less content without diminishing the quality of what the person sees.

When foveation is enabled, the drawable resource for each frame reduces the size of the texture you use for rendering. The drawable also provides rasterization rate maps that specify the amount of rasterization to apply to different parts of the texture. When rendering your scene, the GPU generates fewer pixels in areas with low rasterization rates, and then scales up those areas before displaying them.

## See Also

### Configuring the foveation setting

var generateFlippedRasterizationRateMaps: Bool

A Boolean value that indicates whether the layer renderer provides rasterization rate maps flipped around the y-axis.

