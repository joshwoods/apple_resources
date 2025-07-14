

- Compositor Services
- LayerRenderer
- LayerRenderer.Capabilities
-  supportsFoveation 

Instance Property

# supportsFoveation

A Boolean value that indicates whether the layer supports variable rasterization rates.

visionOS 1.0+

``` source
var supportsFoveation: Bool { get }
```

## Discussion

Foveation support lets you reduce the amount of high-resolution drawing you do. When foveation support is available, the system provides a variable rasterization rate map that defines the content resolution in different parts of the texture. This map allows you to render content in someone’s peripheral vision at a lower resolution than content in the center of their vision.

