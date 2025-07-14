

- RealityKit
- CustomMaterial
-  CustomMaterial.EmissiveColor 

Structure

# CustomMaterial.EmissiveColor

An object that defines the color of the light an entity emits.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct EmissiveColor
```

## Topics

### Creating an emissive color object

init(PhysicallyBasedMaterial.EmissiveColor)

Creates a color of emitted light based on the emissive color property from a physically based material.

init(color: NSColor, texture: CustomMaterial.Texture?)

Creates a color of emitted light in macOS.

init(color: UIColor, texture: CustomMaterial.Texture?)

Creates a color of emitted light in macOS.

### Accessing emissive color data

var texture: CustomMaterial.Texture?

An optional image texture that defines the color of light emission.

var color: UIColor

var color: NSColor

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

