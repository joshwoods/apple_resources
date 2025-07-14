

- RealityKit
- CustomMaterial
-  emissiveColor 

Instance Property

# emissiveColor

The color of light this material emits.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var emissiveColor: CustomMaterial.EmissiveColor { get set }
```

## Discussion

With physically based rendering (PBR), you can give entities in RealityKit the appearance of emitting light. Use this property to simulate real-world objects that glow, such as objects with LEDs or computer screens. To enable light emission from a material, set emissiveIntensity to a value greater than zero, then specify a color (other than black) using this property. You can specify a single emissive color for the entire material, or use a UV-mapped image texture to use different colors for different parts of the entity.

With custom materials, RealityKit doesn’t use emissiveColor automatically to render your entity. Call `params.surface().set_emissive_color()` from your surface shader, otherwise RealityKit renders no light emission.

The following example assigns a tint color to the emissiveColor property, without a texture:

```
self.emissiveColor = PhysicallyBasedMaterial.EmissiveColor(color: .red)
```

This next example uses a texture to specify the emissiveColor property:

```
if let emissiveResource = try? TextureResource.load(named: "entity_emissive") {
    let emissiveMap = MaterialParameters.Texture(emissiveResource)
    material.emissiveColor = .init(texture: emissiveMap)
}
```

This Metal code shows how to access the emissive color tint in your shader functions:

```
half3 emissiveTint = (half3)params.material_constants().emissive_color();
```

The following Metal code demonstrates how to sample the emissive color texture for the current fragment:

```
// Get the entity's primary texture coordinates.
float2 uv = params.geometry().uv0();

// Flip the y-axis. You only need to do this for entities you load from
// USDZ or .reality files.
uv.y = 1.0 - uv.y;

// Sample the emissive color texture to get the value for this fragment.
auto tex = params.textures();
half3 emissiveColor = (half3)tex.emissive_color()
    .sample(textureSampler, uv).rgb;
```

## See Also

### Setting the core properties

var baseColor: CustomMaterial.BaseColor

The color of an entity unmodified by lighting.

var roughness: CustomMaterial.Roughness

The amount the surface of the 3D object scatters reflected light.

var metallic: CustomMaterial.Metallic

The reflectiveness of an entity.

var normal: CustomMaterial.Normal

A texture map that stores fine surface details for the entity.

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

