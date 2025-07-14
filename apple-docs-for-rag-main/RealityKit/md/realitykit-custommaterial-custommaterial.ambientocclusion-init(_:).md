

- RealityKit
- CustomMaterial
- CustomMaterial.AmbientOcclusion
-  init(\_:) 

Initializer

# init(\_:)

Creates an object from a physically based material’s ambient occlusion property.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(_ value: PhysicallyBasedMaterial.AmbientOcclusion)
```

## Parameters 

`value`  

The ambient occlusion property from a PhysicallyBasedMaterial.

## Discussion

Ambient occlusion represents the entity’s exposure to ambient light. This initializer creates a new object by copying the values from an existing PhysicallyBasedMaterial instance’s ambientOcclusion property.

Specify ambient occlusion by using a UV-mapped image called an *ambient occlusion map*. A value of black (`0.0`) represents parts of the model that receive less ambient light because of a crevice, dent, recessed area, or another part of the same entity blocking ambient light from reaching it. Ambient occlusion values of white (`1.0`) represent flat portions of the model that receive full ambient light. You generate ambient occlusion maps by using a 3D software package.

The ambient occlusion texture is available in the material’s surface shader, but RealityKit doesn’t render ambient occlusion unless the surface shader calls `params.surface().set_ambient_occlusion()`.

The following Metal code shows how to use the ambient occlusion texture in a surface shader function:

```
    // Retrieve the entity's texture coordinates.
    float2 uv = params.geometry().uv0();

    // Entities loaded from USDZ or .reality files have texture coordinates
    // with a flipped y-axis. This adjusts for that.
    uv.y = 1.0 - uv.y;

    // Sample the ambient occlusion texture and use it to set the
    // ambient occlusion value to use during rendering.
    auto tex = params.textures();
    half metallic = tex.ambient_occlusion().sample(textureSampler, uv).r;
    params.surface().set_ambient_occlusion(metallic);
```

## See Also

### Creating an ambient occlusion object

init(texture: CustomMaterial.Texture?)

Creates an object from an image texture.

