

- RealityKit
-  PhysicallyBasedMaterial 

Structure

# PhysicallyBasedMaterial

A material that simulates the appearance of real-world objects.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct PhysicallyBasedMaterial
```

## Mentioned in 

Applying realistic material and lighting effects to entities

Modifying RealityKit rendering using custom materials

## Overview

In RealityKit, a *material* is an object that defines the surface properties of a rendered 3D object. A Physically Based Rendering (PBR) material is a material that closely approximates the way light reflects off of real-world objects. Use PhysicallyBasedMaterial to create highly realistic-looking objects for your AR scenes.

Many of the properties for PhysicallyBasedMaterial provide the option to use more than one type of data to specify that property. You can set an object’s baseColor using a specific color for the entire material, or you can use an image that UV-maps on to the entity.

PhysicallyBasedMaterial includes all material properties supported by USDZ. On iOS 15 and later, RealityKit automatically uses PhysicallyBasedMaterial when importing an entity from a USDZ file.

For more information on using PhysicallyBasedMaterial, see Applying realistic material and lighting effects to entities.

## Topics

### Creating a physically based material

init()

Creates a physically based material.

init(program: PhysicallyBasedMaterial.Program)

### Setting the core properties

var baseColor: PhysicallyBasedMaterial.BaseColor

The color of an entity unmodified by lighting.

var roughness: PhysicallyBasedMaterial.Roughness

The amount the surface of the 3D object scatters reflected light.

var metallic: PhysicallyBasedMaterial.Metallic

The reflectiveness of an entity.

var normal: PhysicallyBasedMaterial.Normal

The normal map for the entity.

var ambientOcclusion: PhysicallyBasedMaterial.AmbientOcclusion

The ambient occlusion values for a material.

var specular: PhysicallyBasedMaterial.Specular

The specular highlight applied to the entity.

var clearcoat: PhysicallyBasedMaterial.Clearcoat

The transparent highlights that simulate a clear, shiny coating on an entity.

var clearcoatRoughness: PhysicallyBasedMaterial.ClearcoatRoughness

The degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

var clearcoatNormal: PhysicallyBasedMaterial.ClearcoatNormal

Waviness and imperfections for the top clearcoat.

### Configuring transparency and highlights

var blending: PhysicallyBasedMaterial.Blending

The transparency of an entity.

var sheen: PhysicallyBasedMaterial.SheenColor?

The intensity of an entity’s sheen.

### Adding anisotropy

var anisotropyLevel: PhysicallyBasedMaterial.AnisotropyLevel

The degree to which an entity reflects light to create stretched or oblong highlights.

var anisotropyAngle: PhysicallyBasedMaterial.AnisotropyAngle

The angle at which the anisotropic direction of the material is oriented, influencing the reflection and appearance of surface highlights.

### Adding light emission

var emissiveIntensity: Float

The intensity of light emitted by the entity.

var emissiveColor: PhysicallyBasedMaterial.EmissiveColor

The color of the light the entity emits.

### Modifying texture coordinates

var textureCoordinateTransform: PhysicallyBasedMaterial.TextureCoordinateTransform

A two-dimensional transformation to apply to the entity’s primary texture coordinates.

var secondaryTextureCoordinateTransform: PhysicallyBasedMaterial.TextureCoordinateTransform

A two-dimensional transformation to apply to the entity’s secondary texture coordinates.

### Culling unnecessary polygons

var faceCulling: PhysicallyBasedMaterial.FaceCulling

A process in which the system specifies polygons to remove before rendering a mesh using this material.

### Setting depth testing properties

var readsDepth: Bool

A boolean value that determines whether this material performs the depth test by reading RealityKit’s depth buffer.

var writesDepth: Bool

A boolean value that determines whether this material writes its depth into RealityKit’s depth buffer.

### Setting shader properties

var program: PhysicallyBasedMaterial.Program

### Classes

class Program

An object that represents the backing shader compilation required for physically based materials.

### Structures

struct AmbientOcclusion

An object that defines the ambient occlusion of an entity’s surface.

struct AnisotropyAngle

An object used to define a material’s anisotropy angle.

struct AnisotropyLevel

An object that defines the degree to which an entity reflects light to create stretched or oblong highlights.

struct BaseColor

An object that defines an entity’s base color.

struct Clearcoat

An object that defines the intensity of an entity’s clear, shiny coating.

struct ClearcoatNormal

An object that defines the clearcoat normal map texture.

struct ClearcoatRoughness

An object that defines the degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

struct EmissiveColor

An object that defines the color of the light an entity emits.

struct Metallic

An object that defines the reflectiveness of an entity.

struct Normal

An object that specifies an entity’s normal map.

struct Opacity

An object that defines the opacity of an entity.

struct Roughness

An object that defines the roughness of an entity’s surface.

struct SheenColor

An object that defines the color of an entity’s sheen.

struct Specular

An object that defines the specular highlights of an entity.

### Instance Properties

var opacityThreshold: Float?

A threshold below which RealityKit ignores opacity.

var triangleFillMode: PhysicallyBasedMaterial.TriangleFillMode

The object that controls how RealityKit draws triangles.

### Type Aliases

typealias FaceCulling

An alias for the face culling object that’s appropriate for this material class.

typealias Texture

The texture type to use for materials of this class.

typealias TextureCoordinateTransform

An alias for the texture coordinate transform that’s appropriate for this material class.

typealias TriangleFillMode

An alias for the triangle fill mode object that’s appropriate for this material class.

### Enumerations

enum Blending

The object that defines the transparency of an entity.

### Default Implementations

Material Implementations

## Relationships

### Conforms To

- Material

## See Also

### Realistic materials

Applying realistic material and lighting effects to entities

Enhance the appearance of objects in a RealityKit scene with Physically Based Rendering (PBR).

struct BaseColor

An object that defines an entity’s base color.

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

