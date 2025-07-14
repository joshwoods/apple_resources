

- Compositor Services
- LayerRenderer
-  LayerRenderer.Properties 

Structure

# LayerRenderer.Properties

A type that describes the organization of the layer renderer’s textures and the relationships between those textures and the views you use for drawing.

visionOS 1.0+

``` source
struct Properties
```

## Mentioned in 

Drawing fully immersive content using Metal

## Overview

Use the layer’s properties to configure other parts of your app. For example, use them to configure your app’s render pipeline.

You can obtain layer properties directly from your layer. If you don’t yet have the LayerRenderer type, you can create an equivalent set of properties using the initializer for this type.

## Topics

### Creating representative properties

init(configuration: LayerRenderer.Configuration) throws

Creates a set of properties using the specified configuration values.

### Getting view port information

var viewCount: Int

The number of views that you must fill with content.

### Getting the layer’s texture topology

var textureTopologies: [TextureTopology]

The texture topologies available for the layer.

struct TextureTopology

A type that specifies the organization of one of the drawable’s textures.

## Relationships

### Conforms To

- Copyable

## See Also

### Getting the layer renderer properties

var properties: LayerRenderer.Properties

The configured properties of the layer renderer.

