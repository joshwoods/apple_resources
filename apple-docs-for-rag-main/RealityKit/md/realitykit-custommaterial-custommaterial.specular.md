

- RealityKit
- CustomMaterial
-  CustomMaterial.Specular 

Structure

# CustomMaterial.Specular

An object that defines the specular highlights of an entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct Specular
```

## Overview

In physically based rendering (PBR), specular highlights primarily come from the object’s roughness value. RealityKit renders materials that have a low roughness value with specular highlights based on the environment, lighting, and shape of the entity.

For more information on using specular values in a custom material, see specular.

## Topics

### Creating a specular object

init(floatLiteral: Float)

Creates an object from a single value.

init(scale: Float, texture: CustomMaterial.Texture?)

Creates an object from a single value, a UV-mapped texture, or both.

init(PhysicallyBasedMaterial.Specular)

Creates an object from a physically based material’s specular property.

### Accessing specular values

var scale: Float

The specular value for the entire entity or a multiplier for values sampled from the material’s texture.

var texture: CustomMaterial.Texture?

The specular value as a UV-mapped image texture.

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

struct Roughness

An object that defines how the surface of an entity scatters the light it reflects.

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

struct Clearcoat

An object that defines the intensity of an entity’s clear, shiny coating.

struct ClearcoatNormal

An object that defines the clearcoat normal map texture.

struct ResourceStorage

A container for resources that will be encoded into a CustomMaterial’s custom uniforms argument buffer.

typealias TextureCoordinateTransform

The object type that custom material use to hold UV texture coordinates.

