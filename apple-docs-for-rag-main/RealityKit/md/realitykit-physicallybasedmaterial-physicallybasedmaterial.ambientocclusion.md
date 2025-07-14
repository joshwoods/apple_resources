

- RealityKit
- PhysicallyBasedMaterial
-  PhysicallyBasedMaterial.AmbientOcclusion 

Structure

# PhysicallyBasedMaterial.AmbientOcclusion

An object that defines the ambient occlusion of an entity’s surface.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct AmbientOcclusion
```

## Topics

### Creating an ambient occlusion object

init(texture: PhysicallyBasedMaterial.Texture?)

Creates an object from an image texture.

init(CustomMaterial.AmbientOcclusion)

Creates an object from a custom material’s ambient occlusion property.

### Accessing ambient occlusion values

var texture: PhysicallyBasedMaterial.Texture?

The amount of ambient occlusion specified using a UV-mapped image.

static let textureSemantic: TextureResource.Semantic

The intended use of the object’s texture property.

## See Also

### Realistic materials

Applying realistic material and lighting effects to entities

Enhance the appearance of objects in a RealityKit scene with Physically Based Rendering (PBR).

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

