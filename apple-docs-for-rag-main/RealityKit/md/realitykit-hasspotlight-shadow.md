

- RealityKit
- HasSpotLight
-  shadow 

Instance Property

# shadow

The shadow for the spotlight.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
@MainActor @preconcurrency
var shadow: SpotLightComponent.Shadow? { get set }
```

## Discussion

Set this property to `nil` to remove shadows for the light. Set it to an instance of SpotLightComponent.Shadow to create shadows.

