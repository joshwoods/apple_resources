

- RealityKit
- PhysicallyBasedMaterial
-  PhysicallyBasedMaterial.Metallic 

Structure

# PhysicallyBasedMaterial.Metallic

An object that defines the reflectiveness of an entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct Metallic
```

## Overview

Use this struct to specify an entity’s `metallic` property, which specifies the reflectiveness of an entity. For more information, see metallic.

## Topics

### Creating a metallic object

init(floatLiteral: Float)

Creates an object from single value.

init(scale: Float, texture: PhysicallyBasedMaterial.Texture?)

Creates an object from a color or texture.

init(CustomMaterial.Metallic)

Creates a metallic object from a custom material’s metallic property.

### Accessing metallic data

var texture: PhysicallyBasedMaterial.Texture?

The reflectiveness as a UV-mapped image texture.

static let textureSemantic: TextureResource.Semantic

The intended use of the object’s texture property.

var scale: Float

The reflectiveness for the entire entity.

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

struct Normal

An object that specifies an entity’s normal map.

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

