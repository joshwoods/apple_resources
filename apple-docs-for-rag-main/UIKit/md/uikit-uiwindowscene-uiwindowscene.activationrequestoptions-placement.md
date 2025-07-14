

- UIKit
- UIWindowScene
- UIWindowScene.ActivationRequestOptions
-  placement 

Instance Property

# placement

The placement you prefer when the system activates the window scene.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@MainActor @preconcurrency
var placement: (any UIWindowScenePlacement)? { get set }
```

## Discussion

Provide a scene placement to influence how the system positions the scene on activation. Set the value to `nil` to indicate that the system should determine the most appropriate placement.

## See Also

### Positioning windows

protocol UIWindowScenePlacement

The placement of a window scene in the workspace.

struct UIWindowSceneProminentPlacement

A placement that indicates the system should present the window more prominently than others in the space.

struct UIWindowSceneStandardPlacement

A placement that indicates the system should present the window using the default style of the system in the space.

struct UIWindowScenePushPlacement

A placement that indicates the system needs to present the window by pushing it onto another window.

