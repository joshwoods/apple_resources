

- Compositor Services
- LayerRenderer
-  LayerRenderer.Layout 

Enumeration

# LayerRenderer.Layout

Constants that specify the organization of the textures you use for drawing.

visionOS 1.0+

``` source
enum Layout
```

## Topics

### Getting the texture layouts

case dedicated

A layout that assigns a separate texture to each rendered view.

case shared

A layout that uses a single texture to store the content for all rendered views.

case layered

A layout that specifies each view’s content as a slice of a single texture.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the texture layout

var layout: LayerRenderer.Layout

The layout being used by the layer.

