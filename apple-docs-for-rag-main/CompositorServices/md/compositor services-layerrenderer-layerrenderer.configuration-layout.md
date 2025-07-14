

- Compositor Services
- LayerRenderer
- LayerRenderer.Configuration
-  layout 

Instance Property

# layout

The layout being used by the layer.

visionOS 1.0+

``` source
var layout: LayerRenderer.Layout { get set }
```

## Discussion

Layouts define how Compositor Services creates the color and depth textures it passes to your app. A layout might use separate textures for each view, or combine the content from multiple views into a single texture. The layout type also determines which Metal texture type to create. For more information about the supported layouts, see LayerRenderer.Layout.

## See Also

### Configuring the texture layout

enum Layout

Constants that specify the organization of the textures you use for drawing.

