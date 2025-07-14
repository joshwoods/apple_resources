

- RealityKit
- PhysicallyBasedMaterial
-  PhysicallyBasedMaterial.ClearcoatRoughness 

Structure

# PhysicallyBasedMaterial.ClearcoatRoughness

An object that defines the degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct ClearcoatRoughness
```

## Overview

This object specifies clearcoat roughness for entities that have clearcoat enabled. A clearcoat is a separate layer of transparent specular highlights used to simulate a clear coating, like on a car or the surface of lacquered objects. When you enable clearcoat rendering for a material, RealityKit renders the clearcoat as a separate layer just above the surface of the entity. You can specify a clearcoat roughness value to indicate how much the clearcoat scatters light that bounces off of it, which softens and spreads out the highlights.

## Topics

### Creating a clearcoat roughness object

init(floatLiteral: Float)

Creates a clearcoat roughness object using a single value.

init(scale: Float, texture: PhysicallyBasedMaterial.Texture?)

Creates a clearcoat roughness object using a single value or a texture.

init(CustomMaterial.ClearcoatRoughness)

Creates a clearcoat roughness object from a custom material’s clearcoat roughness property.

### Accessing clearcoat roughness values

var texture: PhysicallyBasedMaterial.Texture?

The clearcoat roughness specified using a UV-mapped image.

static let textureSemantic: TextureResource.Semantic

The intended use of the object’s texture property.

var scale: Float

The clearcoat roughness specified as a single value.

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

struct Specular

An object that defines the specular highlights of an entity.

struct SheenColor

An object that defines the color of an entity’s sheen.

struct Clearcoat

An object that defines the intensity of an entity’s clear, shiny coating.

struct AnisotropyLevel

An object that defines the degree to which an entity reflects light to create stretched or oblong highlights.

struct AnisotropyAngle

An object used to define a material’s anisotropy angle.

struct EmissiveColor

An object that defines the color of the light an entity emits.

typealias TextureCoordinateTransform

An alias for the texture coordinate transform that’s appropriate for this material class.

