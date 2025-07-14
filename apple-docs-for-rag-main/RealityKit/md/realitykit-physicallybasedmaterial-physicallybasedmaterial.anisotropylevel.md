

- RealityKit
- PhysicallyBasedMaterial
-  PhysicallyBasedMaterial.AnisotropyLevel 

Structure

# PhysicallyBasedMaterial.AnisotropyLevel

An object that defines the degree to which an entity reflects light to create stretched or oblong highlights.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct AnisotropyLevel
```

## Overview

By default, PBR materials are isotropic; in other words, an entity that uses PhysicallyBasedMaterial reflects light uniformly in all directions, mimicking the behavior of most real-world objects. Some objects, including those with many small parallel striations such as vinyl records, CDs, or straight hair, reflect light more in some directions than others, resulting in stretched or oblong specular highlights, as shown in the following figure.

Use this object to specify the anisotropyLevel for a material.

## Topics

### Creating an anisotropy level object

init(floatLiteral: Float)

Creates an anisotropy level object from a single value.

init(scale: Float, texture: PhysicallyBasedMaterial.Texture?)

Creates an anisotropy level object using a single value or a texture.

### Accessing anisotropy level values

var texture: PhysicallyBasedMaterial.Texture?

The anisotropy level values specified using a UV-mapped image.

static let textureSemantic: TextureResource.Semantic

The intended use of the object’s texture property.

var scale: Float

The anistropy level specified as a single value.

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

struct ClearcoatRoughness

An object that defines the degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

struct AnisotropyAngle

An object used to define a material’s anisotropy angle.

struct EmissiveColor

An object that defines the color of the light an entity emits.

typealias TextureCoordinateTransform

An alias for the texture coordinate transform that’s appropriate for this material class.

