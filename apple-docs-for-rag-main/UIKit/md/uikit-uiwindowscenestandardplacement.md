

- UIKit
-  UIWindowSceneStandardPlacement 

Structure

# UIWindowSceneStandardPlacement

A placement that indicates the system should present the window using the default style of the system in the space.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
struct UIWindowSceneStandardPlacement
```

## Topics

### Creating a placement

init()

Creates a placement that indicates the system should present the window using the default style of the system in the space.

## Relationships

### Conforms To

- Equatable
- Hashable
- UIWindowScenePlacement

## See Also

### Positioning windows

var placement: (any UIWindowScenePlacement)?

The placement you prefer when the system activates the window scene.

protocol UIWindowScenePlacement

The placement of a window scene in the workspace.

struct UIWindowSceneProminentPlacement

A placement that indicates the system should present the window more prominently than others in the space.

struct UIWindowScenePushPlacement

A placement that indicates the system needs to present the window by pushing it onto another window.

