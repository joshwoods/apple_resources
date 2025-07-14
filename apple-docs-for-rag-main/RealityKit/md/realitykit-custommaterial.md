

- RealityKit
-  CustomMaterial 

Structure

# CustomMaterial

A material that works with custom Metal shader functions.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct CustomMaterial
```

## Mentioned in 

Modifying RealityKit rendering using custom materials

## Overview

Custom, or programmable, materials allow you to leverage RealityKit’s existing shader pipeline to render physically based or unlit materials that support custom Metal shader functions. These functions modify how RealityKit renders an entity. Custom materials support two different types of custom Metal shader functions: geometry modifiers and surface shaders.

Use a \_surface shader \_to calculate or specify all the material attributes that RealityKit uses to render your entity, such as baseColor, normal, and roughness. A *geometry modifier* can offset the position of an entity’s vertices to change the size and shape of an entity. It can also change other per-vertex data, such as vertex color and UV texture coordinates, which define how RealityKit maps textures on to the model.

Important

For the Metal API documentation for custom material shader functions, see the Metal RealityKit APIs PDF.

For more information on creating custom materials and writing shader functions, see Modifying RealityKit rendering using custom materials.

## Topics

### Creating custom materials

init(from: any Material, geometryModifier: CustomMaterial.GeometryModifier) throws

Creates a custom material from an existing material and a geometry modifier.

init(from: any Material, surfaceShader: CustomMaterial.SurfaceShader, geometryModifier: CustomMaterial.GeometryModifier?) throws

Creates a custom material from an existing material, surface shader, and geometry modifier.

init(surfaceShader: CustomMaterial.SurfaceShader, geometryModifier: CustomMaterial.GeometryModifier?, lightingModel: CustomMaterial.LightingModel) throws

Creates a custom material from a lighting model, surface shader, and geometry modifier.

init(program: CustomMaterial.Program)

### Setting the core properties

var baseColor: CustomMaterial.BaseColor

The color of an entity unmodified by lighting.

var roughness: CustomMaterial.Roughness

The amount the surface of the 3D object scatters reflected light.

var metallic: CustomMaterial.Metallic

The reflectiveness of an entity.

var normal: CustomMaterial.Normal

A texture map that stores fine surface details for the entity.

var emissiveColor: CustomMaterial.EmissiveColor

The color of light this material emits.

var ambientOcclusion: CustomMaterial.AmbientOcclusion

The ambient light exposure for a material.

var specular: CustomMaterial.Specular

The bright highlights to apply to the entity.

var clearcoat: CustomMaterial.Clearcoat

The transparent highlights that simulate a clear, shiny coating on an entity.

var clearcoatRoughness: CustomMaterial.ClearcoatRoughness

The degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

var clearcoatNormal: CustomMaterial.ClearcoatNormal

Waviness and imperfections for the top clearcoat.

### Controlling opacity

var opacityThreshold: Float?

The minimum opacity value to treat as fully opaque.

var blending: CustomMaterial.Blending

The transparency of an entity.

### Setting shader properties

var program: CustomMaterial.Program

var custom: CustomMaterial.Custom

User-defined properties for the material’s shader functions.

var lightingModel: CustomMaterial.LightingModel

The lighting model that the material uses.

func withMutableUniforms&lt;UniformsType>(ofType: UniformsType.Type, (inout UniformsType, inout CustomMaterial.ResourceStorage&lt;UniformsType>) -> Void)

Calls the given closure with an inout reference to the underlying storage bound to the custom uniforms argument of a surface shader and geometry modifier.

func withMutableUniforms&lt;UniformsType>(ofType: UniformsType.Type, stage: CustomShaderStage, (inout UniformsType, inout CustomMaterial.ResourceStorage&lt;UniformsType>) -> Void)

Calls the given closure with an inout reference to the underlying storage bound to the custom uniforms argument of a surface shader or geometry modifier.

### Modifying texture coordinates

var textureCoordinateTransform: CustomMaterial.TextureCoordinateTransform

A two-dimensional transformation RealityKit applies to the entity’s primary texture coordinates.

var secondaryTextureCoordinateTransform: CustomMaterial.TextureCoordinateTransform

A two-dimensional transformation RealityKit applies to the entity’s secondary texture coordinates.

### Culling unnecessary polygons

var faceCulling: CustomMaterial.FaceCulling

A process in which the system specifies polygons to remove before rendering a mesh using this material.

### Setting depth testing properties

var readsDepth: Bool

A boolean value that determines whether this material performs the depth test by reading RealityKit’s depth buffer.

var writesDepth: Bool

A boolean value that determines whether this material writes its depth into RealityKit’s depth buffer.

### Classes

class Program

An object that represents the backing shader compilation required for custom materials.

### Structures

struct AmbientOcclusion

An object that defines an entity’s exposure to ambient light.

struct BaseColor

An object that defines an entity’s base color.

struct Clearcoat

An object that defines the intensity of an entity’s clear, shiny coating.

struct ClearcoatNormal

An object that defines the clearcoat normal map texture.

struct ClearcoatRoughness

An object that defines the degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

struct Custom

An object that defines the custom properties for the material.

struct CustomMaterialTexture

A texture object that you use to create custom materials.

struct EmissiveColor

An object that defines the color of the light an entity emits.

struct GeometryModifier

The custom material’s optional shader function that can manipulate an entity’s vertex data.

struct Metallic

An object that defines an entity’s reflectiveness.

struct Normal

An object that stores fine surface details for an entity in an image texture.

struct Opacity

An object that defines the transparency options for a custom material.

struct ResourceStorage

A container for resources that will be encoded into a CustomMaterial’s custom uniforms argument buffer.

struct Roughness

An object that defines how the surface of an entity scatters the light it reflects.

struct Specular

An object that defines the specular highlights of an entity.

struct SurfaceShader

The custom material’s surface shader function.

### Instance Properties

var triangleFillMode: CustomMaterial.TriangleFillMode

The object that controls how RealityKit draws triangles.

### Type Aliases

typealias FaceCulling

The type of object used to control the removal of polygons that aren’t visible to the user.

typealias Texture

The object type that custom materials use to hold texture properties.

typealias TextureCoordinateTransform

The object type that custom material use to hold UV texture coordinates.

typealias TriangleFillMode

### Enumerations

enum Blending

An object that specifies the transparency of an entity.

enum LightingModel

An object that defines how the framework renders a custom material.

### Default Implementations

Material Implementations

## Relationships

### Conforms To

- Material

## See Also

### Shaders

struct ShaderGraphMaterial

typealias FaceCulling

An alias for the cull mode object that’s appropriate for this material class.

typealias TriangleFillMode

An alias for the triangle fill mode object that’s appropriate for this material class.

Modifying RealityKit rendering using custom materials

Write Metal shader functions to implement custom rendering effects.

struct SurfaceShader

The custom material’s surface shader function.

struct GeometryModifier

The custom material’s optional shader function that can manipulate an entity’s vertex data.

protocol MaterialFunction

The abstract superclass for objects representing compute functions for RealityKit custom materials .

class Program

An object that represents the backing shader compilation required for custom materials.

struct Descriptor

An object that specifies all parameters necessary to initialize `CustomMaterial` programs

enum CustomShaderStage

