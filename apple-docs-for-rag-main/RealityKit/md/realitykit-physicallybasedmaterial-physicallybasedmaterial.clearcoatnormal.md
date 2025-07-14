

- RealityKit
- PhysicallyBasedMaterial
-  PhysicallyBasedMaterial.ClearcoatNormal 

Structure

# PhysicallyBasedMaterial.ClearcoatNormal

An object that defines the clearcoat normal map texture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ClearcoatNormal
```

## Overview

An entity in RealityKit can display a clearcoat, which is a separate layer of transparent specular highlights used to simulate a clear coating, like on a car or the surface of lacquered objects. Use this object to specify a clearcoat normal and vary the normal used to calculate the clearcoat. This can be used to add imperfections and waviness to the clearcoat layer.

For information, see clearcoatNormal.

## Topics

### Initializers

init(CustomMaterial.ClearcoatNormal)

Creates a clear coat normal object from a custom material’s clear coat normal property.

init(texture: PhysicallyBasedMaterial.Texture?)

Creates an object from a specified texture.

### Instance Properties

var texture: PhysicallyBasedMaterial.Texture?

The material’s clearcoat normal map.

### Type Properties

static let textureSemantic: TextureResource.Semantic

The intended use of the object’s texture property.

