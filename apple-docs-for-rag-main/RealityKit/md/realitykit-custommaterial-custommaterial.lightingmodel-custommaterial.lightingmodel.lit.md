

- RealityKit
- CustomMaterial
- CustomMaterial.LightingModel
-  CustomMaterial.LightingModel.lit 

Case

# CustomMaterial.LightingModel.lit

The entity renders using physically based rendering techniques without a clearcoat.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
case lit
```

## Discussion

A custom material using the CustomMaterial.LightingModel.lit lighting model uses physically based rendering techniques, but doesn’t render a clearcoat. If a CustomMaterial.LightingModel.lit material’s surface shader calls `params.surface().set_clearcoat()` or `params.surface().set_clearcoat_roughness(),` ReallityKit ignores it.

## See Also

### Specifying the lighting model

case clearcoat

The entity renders using physically based rendering techniques with a clearcoat.

case unlit

The entity renders with no light or shadow calculations.

