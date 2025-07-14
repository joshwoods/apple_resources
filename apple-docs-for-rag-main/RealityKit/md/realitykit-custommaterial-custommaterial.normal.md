

- RealityKit
- CustomMaterial
-  CustomMaterial.Normal 

Structure

# CustomMaterial.Normal

An object that stores fine surface details for an entity in an image texture.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct Normal
```

## Overview

*Normal mapping* is a real-time rendering technique that captures fine surface details for a model by using a texture instead of by increasing the number of polygons in the model. It works by storing *surface normals*, which are vectors perpendicular to the surface of the model, from a much higher-resolution version of the same 3D object. A normal map stores each vector in the image by storing the vectors’ `X`, `Y`, and `Z` values as the `R`, `G`, and `B` components of the corresponding pixel in the UV-mapped image. This object defines a normal map for a custom material.

For more information on using normal map values in a custom material, see normal.

## Topics

### Creating a normal object

init(texture: CustomMaterial.Texture?)

Create an object from a specified texture.

init(PhysicallyBasedMaterial.Normal)

Creates an object containing surface details for an entity from a custom material’s normal property.

### Accessing the normal map

var texture: CustomMaterial.Texture?

The material’s normal map.

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

