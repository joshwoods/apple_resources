

- Compositor Services
- LayerRenderer
- LayerRenderer.Capabilities
-  supportedColorFormats 

Instance Property

# supportedColorFormats

An array of color formats that the layer supports for its textures.

visionOS 1.0+

``` source
var supportedColorFormats: [MTLPixelFormat] { get }
```

## Discussion

The pixel formats in this property tell you which pixel arrangements and characteristics the layer supports for its color textures.

## See Also

### Getting the supported formats

var supportedDepthFormats: [MTLPixelFormat]

The list of depth formats that the layer supports

