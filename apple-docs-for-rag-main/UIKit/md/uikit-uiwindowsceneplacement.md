

- UIKit
-  UIWindowScenePlacement 

Protocol

# UIWindowScenePlacement

The placement of a window scene in the workspace.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
protocol UIWindowScenePlacement : Hashable
```

## Topics

### Positioning windows

static func prominent() -> Self

Creates a placement that indicates the system should present the window more prominently than others in the space.

static func standard() -> Self

Creates a placement that indicates the system should present the window using the default style of the system in the space.

### Type Methods

static func push(onto: UISceneSession) -> Self

static func replacing(UISceneSession) -> SelfDeprecated

## Relationships

### Inherits From

- Equatable
- Hashable

### Conforming Types

- UIWindowSceneProminentPlacement
- UIWindowScenePushPlacement
- UIWindowSceneReplacePlacement
- UIWindowSceneStandardPlacement

## See Also

### Positioning windows

var placement: (any UIWindowScenePlacement)?

The placement you prefer when the system activates the window scene.

struct UIWindowSceneProminentPlacement

A placement that indicates the system should present the window more prominently than others in the space.

struct UIWindowSceneStandardPlacement

A placement that indicates the system should present the window using the default style of the system in the space.

struct UIWindowScenePushPlacement

A placement that indicates the system needs to present the window by pushing it onto another window.

