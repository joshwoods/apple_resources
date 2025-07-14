

- RealityKit
- CustomMaterial
-  CustomMaterial.Roughness 

Structure

# CustomMaterial.Roughness

An object that defines how the surface of an entity scatters the light it reflects.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct Roughness
```

## Overview

In physically based rendering, the `roughness` property represents how much the surface of an entity scatters the light it reflects. A material with a high roughness has a matte appearance, whereas one with a low roughness has a shiny appearance.

For more information on using roughness values in a custom material, see roughness.

## Topics

### Creating a roughness object

init(floatLiteral: Float)

Creates an object to specify the amount of roughness, using a single value that applies to the entire material.

init(scale: Float, texture: CustomMaterial.Texture?)

Creates a roughness object from a color or texture.

init(PhysicallyBasedMaterial.Roughness)

Creates a roughness object from a physically based material’s roughness property.

### Accessing roughness values

var scale: Float

The roughness value for the entire entity or a multiplier for its texture.

var texture: CustomMaterial.Texture?

The roughness values as a UV-mapped image texture.

typealias FloatLiteralType

A type that represents a floating-point literal.

## Relationships

### Conforms To

- ExpressibleByFloatLiteral

## See Also

### Custom material types

struct Custom

An object that defines the custom properties for the material.

struct CustomMaterialTexture

A texture object that you use to create custom materials.

enum LightingModel

An object that defines how the framework renders a custom material.

struct BaseColor

An object that defines an entity’s base color.

struct Metallic

An object that defines an entity’s reflectiveness.

struct Normal

An object that stores fine surface details for an entity in an image texture.

struct EmissiveColor

An object that defines the color of the light an entity emits.

enum Blending

An object that specifies the transparency of an entity.

struct Opacity

An object that defines the transparency options for a custom material.

struct AmbientOcclusion

An object that defines an entity’s exposure to ambient light.

struct Specular

An object that defines the specular highlights of an entity.

struct Clearcoat

An object that defines the intensity of an entity’s clear, shiny coating.

struct ClearcoatNormal

An object that defines the clearcoat normal map texture.

struct ResourceStorage

A container for resources that will be encoded into a CustomMaterial’s custom uniforms argument buffer.

typealias TextureCoordinateTransform

The object type that custom material use to hold UV texture coordinates.

