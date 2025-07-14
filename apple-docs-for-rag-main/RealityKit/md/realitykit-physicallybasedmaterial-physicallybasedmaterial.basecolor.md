

- RealityKit
- PhysicallyBasedMaterial
-  PhysicallyBasedMaterial.BaseColor 

Structure

# PhysicallyBasedMaterial.BaseColor

An object that defines an entity’s base color.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct BaseColor
```

## Overview

Use this struct to specify an entity’s base color, which defines the entity’s appearance before RealityKit calculates the effect of lighting or material properties such as roughness or metallic. For more information, see baseColor.

## Topics

### Creating a base color object

init(tint: UIColor, texture: MaterialParameters.Texture?)

Creates a base color object from a color or texture on macOS.

init(tint: NSColor, texture: MaterialParameters.Texture?)

Creates a base color object from a color or texture on macOS.

init(CustomMaterial.BaseColor)

Creates a base color object from a custom material’s base color property.

### Accessing texture data

var texture: PhysicallyBasedMaterial.Texture?

The base color as a UV Image map.

static let textureSemantic: TextureResource.Semantic

The intended use of this object’s texture property.

### Instance Properties

var tint: UIColor

var tint: NSColor

## See Also

### Realistic materials

Applying realistic material and lighting effects to entities

Enhance the appearance of objects in a RealityKit scene with Physically Based Rendering (PBR).

struct PhysicallyBasedMaterial

A material that simulates the appearance of real-world objects.

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

struct AnisotropyLevel

An object that defines the degree to which an entity reflects light to create stretched or oblong highlights.

struct AnisotropyAngle

An object used to define a material’s anisotropy angle.

struct EmissiveColor

An object that defines the color of the light an entity emits.

typealias TextureCoordinateTransform

An alias for the texture coordinate transform that’s appropriate for this material class.

