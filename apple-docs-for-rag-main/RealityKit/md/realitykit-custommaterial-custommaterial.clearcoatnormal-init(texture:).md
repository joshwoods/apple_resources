

- RealityKit
- CustomMaterial
- CustomMaterial.ClearcoatNormal
-  init(texture:) 

Initializer

# init(texture:)

Construct a `CustomMaterial.ClearcoatNormal` object from a texture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
init(texture: CustomMaterial.Texture? = nil)
```

## Parameters 

`texture`  

The clearcoat normals as the texture of a UV-mapped image.

## Discussion

```
if let textureResource = try? TextureResource.load(named: "entity_cc_normalMap") {
    let ccNormalMap = CustomMaterial.Texture(textureResource)
    let clearcoatNormal = CustomMaterial.ClearcoatNormal(texture: ccNormalMap)
}
```

