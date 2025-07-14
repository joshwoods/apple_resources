

- RealityKit
- CustomMaterial
-  CustomMaterial.Custom 

Structure

# CustomMaterial.Custom

An object that defines the custom properties for the material.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct Custom
```

## Topics

### Creating a custom object

init(value: SIMD4&lt;Float>, texture: CustomMaterial.Texture?)

Creates a custom object from a vector and texture.

### Accessing custom values

var value: SIMD4&lt;Float>

A custom vector that the framework sends to the material’s shader functions.

var texture: CustomMaterial.Texture?

A custom UV-mapped image texture that the framework sends to the material’s shader functions.

## See Also

### Custom material types

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

struct Clearcoat

An object that defines the intensity of an entity’s clear, shiny coating.

struct ClearcoatNormal

An object that defines the clearcoat normal map texture.

struct ResourceStorage

A container for resources that will be encoded into a CustomMaterial’s custom uniforms argument buffer.

typealias TextureCoordinateTransform

The object type that custom material use to hold UV texture coordinates.

