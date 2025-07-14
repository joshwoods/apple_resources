

- RealityKit
- Materials, textures, and shaders
-  Applying realistic material and lighting effects to entities 

Article

# Applying realistic material and lighting effects to entities

Enhance the appearance of objects in a RealityKit scene with Physically Based Rendering (PBR).

## Overview

A Material instance describes the surface properties of an entity and controls how RealityKit renders that entity. A PhysicallyBasedMaterial is a type of material that closely approximates the way light bounces off objects in the real world. It creates very realistic rendered objects that look natural when placed into an AR scene.

When you import models from USDZ files, RealityKit automatically creates one or more PhysicallyBasedMaterial instances from the PBR material settings in the file. You can also create PBR materials manually, either to change the appearance of an entity loaded from a USDZ file at runtime, or to use PBR rendering with procedurally created entities.

### Create a material and specify core properties

PBR materials use three core properties to define an object’s fundamental appearance: baseColor, roughness, and metallic. The baseColor property defines the underlying color of the entity as it would look under soft, bright, neutral lighting with no shadows or highlights. The `roughness` property is a measure of how the surface of the entity scatters the light that it reflects. A material with a low `roughness` looks shiny, while one with a high `roughness` has a matte appearance. The `metallic` property defines how the material reflects the environment around the entity. The figure below illustrates the visual effects of changing the metallic and roughness values of a PhysicallyBasedMaterial while keeping its baseColor unchanged.

This example demonstrates how to create a PBR material that uses a color and a single `roughness` and `metallic` value for the entire material:

```
var material = PhysicallyBasedMaterial()
material.baseColor.tint = .orange
material.roughness = PhysicallyBasedMaterial.Roughness(
    floatLiteral: 0.0
)
material.metallic = PhysicallyBasedMaterial.Metallic(
    floatLiteral: 1.0
)
```

And the following example shows how to create a PBR material using UV-mapped image textures for all three properties:

```
var material = PhysicallyBasedMaterial()

if let baseResource = try? TextureResource.load(named: "entity_basecolor") {
    let baseTexture = MaterialParameters.Texture(baseResource)
    material.baseColor = PhysicallyBasedMaterial.BaseColor(
        texture: baseTexture
    )
}

if let metalResource = try? TextureResource.load(named: "entity_metallic") {
    let metalTexture = MaterialParameters.Texture(metalResource)
    material.metallic = PhysicallyBasedMaterial.Metallic(
        texture: metalTexture
    )
}

if let roughnessResource = try? TextureResource.load(named: "entity_roughness") {
    let roughnessTexture = MaterialParameters.Texture(roughnessResource)
    material.roughness = PhysicallyBasedMaterial.Roughness(
        texture: roughnessTexture
    )
}
```

For metallic and roughness maps, use a grayscale image. If you use a color image, RealityKit only uses the red channel.

### Add a normal map

*Normal mapping* is a real-time rendering technique that captures fine surface details for a model using a texture instead of increasing the number of polygons in the model. It works by storing *surface normals*, which are vectors perpendicular to the surface of the model, from a much higher resolution version of the same 3D object. A normal map stores vectors by storing its `X`, `Y`, and `Z` value as the `R`, `G`, and `B` components of the corresponding pixel in a UV-mapped image. RealityKit uses those normals to do lighting calculations, which results in much more realistic highlights, shadows, and reflections without incurring the computational cost of using a much higher resolution 3D model.

RealityKit’s `PhysicallyBasedMaterial` supports normal maps using the normal property.

Note

RealityKit uses *tangent space normal maps,* which many 3D software packages can create. You can recognize tangent space normal maps by their predominately purple color.

To add a `normal` map to your entity, load it as a texture resource, and use the resource to create a `PhysicallyBasedMaterial.Normal` instance, as in this example:

```
if let normalResource = try? TextureResource.load(named: "entity_normals") {
    let normalTexture = MaterialParameters.Texture(normalResource)
    material.normal = PhysicallyBasedMaterial.Normal(
        texture: normalTexture
    )
}
```

### Specify blending and opacity

By default, RealityKit materials are opaque, but RealityKit can render entities with transparency to simulate real-world objects. To render a material with transparency, change the blending value from `.opaque` to `.transparent`. The `.transparent` enumeration case takes an associated value that controls the amount of transparency.

To specify opacity, create a `PhysicallyBasedMaterial.Opacity` object. You can specify opacity for the entire entity using a single value between `0.0` and `1.0`, where `1.0` is fully opaque and `0.0` is fully transparent.

```
material.blending = .transparent(
    opacity: PhysicallyBasedMaterial.Opacity(floatLiteral: 0.5)
)
```

You can also specify opacity using an image texture (sometimes called an *alpha map* or *transparency map*). In an alpha map, black pixels represent fully transparent parts of the entity, white pixels represent fully opaque parts of the entity, and gray pixels represent parts of the entity that are partially transparent.

```
if let opacityResource = try? TextureResource.load(named: "entity_opacity") {
    let opacityMap = MaterialParameters.Texture(opacityResource)
    let opacityValue = PhysicallyBasedMaterial.Opacity(texture: opacityMap)
    material.blending = .transparent(opacity: opacityValue)
}
```

You can change the behavior of an alpha map to function as a *mask* rather than a transparency map. When using an alpha mask, RealityKit draws every pixel of the entity either fully transparent or fully opaque with no partially transparency. Use the opacityThreshold property to enable alpha masking. If you specify a value greater than `0.0`, RealityKit uses the image texture as a mask, and renders any pixel with a value of less than or equal to opacityThreshold as fully transparent. RealityKit draws any pixel value greater than opacityThreshold as fully opaque.

### Add specular highlights

RealityKit automatically draws *specular highlights* for physically based materials using the values of various properties, primarily roughness and metallic. Specular highlights are bright spots of reflected light that appear on shiny objects.

While many real-world objects can be accurately and realistically simulated with just the core PBR properties, you can create additional realistic effects by augmenting the specular highlights.

Use the specular property to simulate the bright highlights found on certain *dielectric* (nonmetallic) materials like cut gemstones and faceted glass, which have specular highlights much brighter than the ones RealityKit creates from just the core properties.

Here’s how to specify specular using a single value for the entire material:

```
material.specular = PhysicallyBasedMaterial.Specular(
    floatLiteral: 0.8
)
```

The following example demonstrates how to specify specular using a UV-mapped image texture:

```
if let specularResource = try? TextureResource.load(named: "entity_specular") {
    let specularTexture = MaterialParameters.Texture(specularResource)
    material.specular = PhysicallyBasedMaterial.Specular(
        texture: specularTexture
    )
}
```

You can also use specular highlights to simulate subtle reflections like the ones that occur on some types of fabric. Create these types of effects with the sheen property, as illustrated in the following figure.

This example shows how to specify sheen using a single value for the entire material:

```
let sheenTint = PhysicallyBasedMaterial.Color(
    red: 0.8, green: 0.8, blue: 0.8, alpha: 1.0
)
material.sheen = PhysicallyBasedMaterial.SheenColor(
    tint: sheenTint
)
```

And this example demonstrates how to specify sheen using a UV-mapped image texture:

```
if let sheenResource = try? TextureResource.load(named: "entity_sheen") {
    let sheenMap = MaterialParameters.Texture(sheenResource)
    material.sheen = PhysicallyBasedMaterial.SheenColor(
        texture: sheenMap
    )
}
```

### Use anisotropy for directional highlights

By default, PBR materials are *isotropic*; in other words, an entity that uses a PhysicallyBasedMaterial reflects light uniformly in all directions, mimicking the behavior of most real-world objects. Some objects, including those with many small parallel striations such as vinyl records, CDs, or straight hair, reflect light more in some directions than others, resulting in stretched or oblong specular highlights called *anisotropic* highlights.

In RealityKit, you adjust anisotropy using two parameters: anisotropyLevel and anisotropyAngle. To control the amount of anisotropy, use anisotropyLevel. Specifying a value of `0.0` results in an entirely isotropic appearance, while nonzero values up to `1.0` simulate the appearance of increasingly anisotropic objects. Change the angle of anisotropy to affect the direction in which the specular highlights stretch with anisotropyAngle, which also takes a value between `0.0 `and `1.0.` `A` value of `0.0` means a rotation of 0° and a value of `1.0` indicates a rotation of 360°. To determine the anisotropyAngle value to use, divide the desired angle in degrees by `360.0` or the desired angle in radians by pi times 2.

```
let angleDegrees: Float = 125
let anisotropyAngleFromDegrees = angleDegrees / 360

let angleRadians: Float = 2.181662
let anisotropyAngleFromRadians = angleRadians / (2 * .pi)
```

The following example demonstrates how to specify anisotropy using single values for the entire material:

```
material.anisotropyLevel = PhysicallyBasedMaterial.AnisotropyLevel(
    floatLiteral: 0.5
)
material.anisotropyAngle = PhysicallyBasedMaterial.AnisotropyAngle(
    floatLiteral: 0.5
)
```

And this example shows how to specify anisotropy using a UV-mapped image texture for anisotropyLevel and a separate image for anisotropyAngle:

```
if let anisoLevelResource = try? TextureResource.load(named: "entity_aniso_level") {
    let anisoLevelMap = MaterialParameters.Texture(anisoLevelResource)
    material.anisotropyLevel = PhysicallyBasedMaterial.AnisotropyLevel(
        texture: anisoLevelMap
    )
}

if let anisoAngleResource = try? TextureResource.load(named: "entity_aniso_angle") {
    let anisoAngleMap = MaterialParameters.Texture(anisoAngleResource)
    material.anisotropyAngle = PhysicallyBasedMaterial.AnisotropyAngle(
        texture: anisoAngleMap
    )
}
```

## See Also

### Realistic materials

struct PhysicallyBasedMaterial

A material that simulates the appearance of real-world objects.

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

