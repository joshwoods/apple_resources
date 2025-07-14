

- RealityKit
- DirectionalLight
-  shadow 

Instance Property

# shadow

The shadow settings for a directional light.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
@MainActor @preconcurrency
var shadow: DirectionalLightComponent.Shadow? { get set }
```

## Discussion

Set this value to `nil` to remove shadows.

## See Also

### Configuring the directional light

var light: DirectionalLightComponent

A directional light component for the entity.

