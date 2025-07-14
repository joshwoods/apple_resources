

- RealityKit
- PhysicallyBasedMaterial
-  PhysicallyBasedMaterial.Normal 

Structure

# PhysicallyBasedMaterial.Normal

An object that specifies an entity’s normal map.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct Normal
```

## Overview

The `normal` property of a RealityKit entity holds an optional *normal map*, which stores fine details about the entity’s surface, using a texture rather than increasing the number of polygons in the model. If you provide a normal map, RealityKit uses the vectors from that normal map when rendering the entity, resulting in greater detail and more accurate highlights, shadows, and reflections.

## Topics

### Creating a normal object

init(texture: PhysicallyBasedMaterial.Texture?)

Creates an object from a specified texture.

init(CustomMaterial.Normal)

Creates a normal object from a custom material’s normal property.

### Accessing the normal map

var texture: PhysicallyBasedMaterial.Texture?

The material’s normal map.

static let textureSemantic: TextureResource.Semantic

The intended use of the object’s texture property.

## See Also

### Realistic materials

Applying realistic material and lighting effects to entities

Enhance the appearance of objects in a RealityKit scene with Physically Based Rendering (PBR).

struct PhysicallyBasedMaterial

A material that simulates the appearance of real-world objects.

struct BaseColor

An object that defines an entity’s base color.

struct Roughness

An object that defines the roughness of an entity’s surface.

struct Metallic

An object that defines the reflectiveness of an entity.

enum Blending

The object that defines the transparency of an entity.

struct AmbientOcclusion

An object that defines the ambient occlusion of an entity’s surface.

struct Specular

An object that defines the specular highlights of an entity.

struct SheenColor

An object that defines the color of an entity’s sheen.

struct Clearcoat

An object that defines the intensity of an entity’s clear, shiny coating.

struct ClearcoatRoughness

An object that defines the degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

struct AnisotropyLevel

An object that defines the degree to which an entity reflects light to create stretched or oblong highlights.

struct AnisotropyAngle

An object used to define a material’s anisotropy angle.

struct EmissiveColor

An object that defines the color of the light an entity emits.

typealias TextureCoordinateTransform

An alias for the texture coordinate transform that’s appropriate for this material class.

