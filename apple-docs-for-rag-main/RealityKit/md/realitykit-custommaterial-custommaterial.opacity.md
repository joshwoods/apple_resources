

- RealityKit
- CustomMaterial
-  CustomMaterial.Opacity 

Structure

# CustomMaterial.Opacity

An object that defines the transparency options for a custom material.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct Opacity
```

## Topics

### Creating an opacity object

init(floatLiteral: Float)

Creates an opacity object from a single value.

init(scale: Float, texture: CustomMaterial.Texture?)

Creates an object that defines the opacity of an entity using a single value, a UV-mapped image texture, or both.

init(PhysicallyBasedMaterial.Opacity)

Creates an object from the opacity property of an existing physically based material.

### Accessing opacity data

var scale: Float

The amount of opacity specified as a single value.

var texture: CustomMaterial.Texture?

The amount of opacity specified using a UV-mapped image.

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

