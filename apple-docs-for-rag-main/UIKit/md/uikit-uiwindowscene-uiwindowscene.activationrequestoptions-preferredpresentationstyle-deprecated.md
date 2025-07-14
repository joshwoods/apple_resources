

- UIKit
- UIWindowScene
- UIWindowScene.ActivationRequestOptions
-  preferredPresentationStyle Deprecated

Instance Property

# preferredPresentationStyle

The presentation style of the window scene.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedtvOS 15.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var preferredPresentationStyle: UIWindowScene.PresentationStyle { get set }
```

Deprecated

Use placement (Swift) or placement (Objective-C) instead.

## Discussion

The presentation style determines how the system displays the new window scene relative to other scenes in the workspace. The default style is UIWindowScene.PresentationStyle.automatic.

## See Also

### Deprecated

struct UIWindowSceneReplacePlacementDeprecated

