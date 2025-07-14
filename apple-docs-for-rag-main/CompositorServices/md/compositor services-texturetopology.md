

- Compositor Services
-  TextureTopology 

Structure

# TextureTopology

A type that specifies the organization of one of the drawable’s textures.

visionOS 1.0+

``` source
struct TextureTopology
```

## Overview

Metal supports multiple organizations for the textures you use for drawing. Use this type to identify one of the organizations available to use in your app.

## Topics

### Getting the topology type

var textureType: MTLTextureType

The texture type value that specifies how the underlying texture organizes its views.

### Getting the array length

var arrayLength: UInt64

The number of items in the texture array.

### Creating a topology

init()

Creates a texture topology.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Getting the layer’s texture topology

var textureTopologies: [TextureTopology]

The texture topologies available for the layer.

