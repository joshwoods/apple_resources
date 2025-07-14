

- RealityKit
- CustomMaterial
-  CustomMaterial.Clearcoat 

Structure

# CustomMaterial.Clearcoat

An object that defines the intensity of an entity’s clear, shiny coating.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct Clearcoat
```

## Topics

### Creating a clearcoat object

init(floatLiteral: Float)

Creates a clearcoat object using a single value.

init(scale: Float, texture: CustomMaterial.Texture?)

Creates a clearcoat object using a single value or a texture.

init(PhysicallyBasedMaterial.Clearcoat)

Creates a custom clearcoat object from a physically based material’s clearcoat property.

### Accessing clearcoat values

var scale: Float

The intensity of the clearcoat.

var texture: CustomMaterial.Texture?

The clearcoat intensity specified using a UV-mapped image.

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

struct Specular

An object that defines the specular highlights of an entity.

struct ClearcoatNormal

An object that defines the clearcoat normal map texture.

struct ResourceStorage

A container for resources that will be encoded into a CustomMaterial’s custom uniforms argument buffer.

typealias TextureCoordinateTransform

The object type that custom material use to hold UV texture coordinates.

