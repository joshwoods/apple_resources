

- RealityKit
- CustomMaterial
-  CustomMaterial.BaseColor 

Structure

# CustomMaterial.BaseColor

An object that defines an entity’s base color.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct BaseColor
```

## Mentioned in 

Modifying RealityKit rendering using custom materials

## Overview

For more information on using base color values in a custom material, see baseColor.

## Topics

### Creating a base color object

init(tint: UIColor, texture: CustomMaterial.Texture?)

Creates a base color object from a color or texture on macOS.

init(tint: NSColor, texture: CustomMaterial.Texture?)

Creates a base color object from a color or texture on macOS.

init(PhysicallyBasedMaterial.BaseColor)

Creates a custom base color object from an existing physically based material’s base color object.

### Accessing base color data

var texture: CustomMaterial.Texture?

The base color as a UV-mapped image.

var tint: UIColor

var tint: NSColor

## See Also

### Custom material types

struct Custom

An object that defines the custom properties for the material.

struct CustomMaterialTexture

A texture object that you use to create custom materials.

enum LightingModel

An object that defines how the framework renders a custom material.

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

