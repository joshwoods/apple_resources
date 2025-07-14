

- Model I/O
- MDLMaterialSemantic
-  MDLMaterialSemantic.anisotropicRotation 

Case

# MDLMaterialSemantic.anisotropicRotation

The angle at which anisotropic effects are rotated relative to the local tangent basis.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
case anisotropicRotation
```

## Discussion

Values for this semantic in the range from `0.0` to `1.0` map to angles from `0.0` to `2 * M_PI`. This semantic has no effect in a mesh that does not contain vertex attribute data providing a tangent basis.

Model I/O uses this semantic for the `anisotropicRotation` and `map_anisotropicRotation` attributes when importing from the MTL file format (for assets in the OBJ file format).

## See Also

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

