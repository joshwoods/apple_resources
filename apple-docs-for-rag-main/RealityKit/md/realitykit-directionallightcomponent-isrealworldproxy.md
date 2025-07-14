

- RealityKit
- DirectionalLightComponent
-  isRealWorldProxy 

Instance Property

# isRealWorldProxy

A Boolean that you use to control whether the directional light operates as a proxy for a real-world light.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
var isRealWorldProxy: Bool
```

## Discussion

Set the value to `true` when you want the light to cast shadows on virtual content without illuminating anything in the scene. You can use this to create shadows on occlusion materials that accept dynamic lighting.

## See Also

### Setting intensity and shadows

var intensity: Float

The intensity of the directional light, measured in lumen per square meter.

