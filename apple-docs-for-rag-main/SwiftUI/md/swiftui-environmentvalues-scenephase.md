

- SwiftUI
- EnvironmentValues
-  scenePhase 

Instance Property

# scenePhase

The current phase of the scene.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var scenePhase: ScenePhase { get set }
```

## Discussion

The system sets this value to provide an indication of the operational state of a scene or collection of scenes. The exact meaning depends on where you access the value. For more information, see ScenePhase.

## See Also

### Monitoring scene life cycle

enum ScenePhase

An indication of a scene’s operational state.

