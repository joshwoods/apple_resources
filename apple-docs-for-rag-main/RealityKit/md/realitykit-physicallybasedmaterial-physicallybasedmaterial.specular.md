

- RealityKit
- PhysicallyBasedMaterial
-  PhysicallyBasedMaterial.Specular 

Structure

# PhysicallyBasedMaterial.Specular

An object that defines the specular highlights of an entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct Specular
```

## Overview

RealityKit automatically draws *specular highlights* for physically based materials, using the values of various properties, primarily roughness and metallic. Specular highlights are bright spots of reflected light that appear on shiny objects.

Although many real-world objects can be accurately and realistically simulated with just the core physically based rendering (PBR) properties, you can create additional realistic effects by augmenting the specular highlights.

Use this object to specify the amount of specular for a PhysicallyBasedMaterial.

## Topics

### Creating a specular object

init(floatLiteral: Float)

Creates an object from single value.

init(scale: Float, texture: PhysicallyBasedMaterial.Texture?)

Creates an object from a single value or a texture.

init(CustomMaterial.Specular)

Creates an object from a custom material’s specular property.

### Accessing specular values

var texture: PhysicallyBasedMaterial.Texture?

The amount of specular as a UV-mapped image texture.

static let textureSemantic: TextureResource.Semantic

The intended use of the object’s texture property.

var scale: Float

The amount of specular for the entire entity.

typealias FloatLiteralType

A type that represents a floating-point literal.

## Relationships

### Conforms To

- ExpressibleByFloatLiteral

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

struct Normal

An object that specifies an entity’s normal map.

enum Blending

The object that defines the transparency of an entity.

struct AmbientOcclusion

An object that defines the ambient occlusion of an entity’s surface.

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

