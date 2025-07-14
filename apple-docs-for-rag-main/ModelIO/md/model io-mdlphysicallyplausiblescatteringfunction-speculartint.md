

- Model I/O
- MDLPhysicallyPlausibleScatteringFunction
-  specularTint 

Instance Property

# specularTint

The balance of color for specular highlights, between the light color (lower values) and the material’s base color (at higher values).

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var specularTint: MDLMaterialProperty { get }
```

## Discussion

The default value is zero—specular highlights entirely use the color of the reflected light source.

## See Also

### Working with Shading Properties

var subsurface: MDLMaterialProperty

The degree to which light scatters under the surface of the material.

var metallic: MDLMaterialProperty

The degree to which the material appears as a dielectric surface (lower values) or as a metal (higher values).

var specularAmount: MDLMaterialProperty

The tendency of the material to generate specular highlights.

var roughness: MDLMaterialProperty

The degree to which a material appears smooth, affecting both diffuse and specular response.

var anisotropic: MDLMaterialProperty

The degree to which specular highlights elongate in the direction of the local tangent basis.

var anisotropicRotation: MDLMaterialProperty

The angle at which anisotropic effects are rotated relative to the local tangent basis.

var sheen: MDLMaterialProperty

The intensity of highlights that appear only at glancing angles on a material’s surface.

var sheenTint: MDLMaterialProperty

The balance of color for highlights that appear only at glancing angles, between the light color (lower values) and the material’s base color (at higher values).

var clearcoat: MDLMaterialProperty

The intensity of a second specular highlight, similar to the gloss that results from a clear coat on an automotive finish.

var clearcoatGloss: MDLMaterialProperty

The sharpness of a second specular highlight, similar to the gloss that results from a clear coat on an automotive finish.

