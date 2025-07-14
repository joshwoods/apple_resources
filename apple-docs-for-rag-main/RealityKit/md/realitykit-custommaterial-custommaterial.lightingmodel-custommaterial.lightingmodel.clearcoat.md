

- RealityKit
- CustomMaterial
- CustomMaterial.LightingModel
-  CustomMaterial.LightingModel.clearcoat 

Case

# CustomMaterial.LightingModel.clearcoat

The entity renders using physically based rendering techniques with a clearcoat.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
case clearcoat
```

## Discussion

A custom material using the CustomMaterial.LightingModel.clearcoat lighting model uses physically based rendering, including a clearcoat if the material’s surface shader calls `params.surface().set_clearcoat()`.

## See Also

### Specifying the lighting model

case lit

The entity renders using physically based rendering techniques without a clearcoat.

case unlit

The entity renders with no light or shadow calculations.

