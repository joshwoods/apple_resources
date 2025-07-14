

- Model I/O
-  MDLMaterialSemantic 

Enumeration

# MDLMaterialSemantic

Options for the semantic use of a material property’s value in rendering a particular surface appearance; used by the semantic property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
enum MDLMaterialSemantic
```

## Topics

### Constants

case baseColor

The inherent color of a surface, to be used as a modulator during shading.

case subsurface

The degree to which light scatters under the surface of a material.

case metallic

The degree to which a material appears as a dielectric surface (lower values) or as a metal (higher values).

case specular

The intensity of specular highlights that appear on the material’s surface.

case specularExponent

The exponent to be used in Blinn-Phong approximation of the material’s specular response.

case specularTint

The balance of color for specular highlights, between the light color (lower values) and the material’s base color (at higher values).

case roughness

The degree to which a material appears smooth, affecting both diffuse and specular response.

case anisotropic

The degree to which specular highlights elongate in the direction of the local tangent basis.

case anisotropicRotation

The angle at which anisotropic effects are rotated relative to the local tangent basis.

case sheen

The intensity of highlights that appear only at glancing angles on a material’s surface.

case sheenTint

The balance of color for highlights that appear only at glancing angles, between the light color (lower values) and the material’s base color (at higher values).

case clearcoat

The intensity of a second specular highlight, similar to the gloss that results from a clear coat on an automotive finish.

case clearcoatGloss

The spread of a second specular highlight, similar to the gloss that results from a clear coat on an automotive finish.

case emission

The color emitted as radiance from a material’s surface.

case bump

The degree of perturbation in a material’s surface.

case opacity

The opacity of a material’s surface.

case interfaceIndexOfRefraction

The index of refraction for the medium surrounding a material.

case materialIndexOfRefraction

The index of refraction for a material itself.

case objectSpaceNormal

The variation in the surface normal vectors in a material, relative to model coordinate space.

case tangentSpaceNormal

The variation in the surface normal vectors in a material, relative to surface tangent coordinate space.

case displacement

The displacement of a material’s surface relative to the surface normal.

case displacementScale

The scaling factor for displacement of a material’s surface.

case ambientOcclusion

The attenuation of ambient light due to local geometry variations on a surface.

case ambientOcclusionScale

The scaling factor for ambient occlusion shading.

case none

The material property’s semantic property has not been initialized.

case userDefined

The meaning of the material property’s value is not one of the standard semantic uses recognized by Model I/O.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum MDLMaterialPropertyType

Options for the data type of a material property, used by the type property.

