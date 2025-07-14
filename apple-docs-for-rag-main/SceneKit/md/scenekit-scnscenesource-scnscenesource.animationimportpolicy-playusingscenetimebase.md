

- SceneKit
- SCNSceneSource
- SCNSceneSource.AnimationImportPolicy
-  playUsingSceneTimeBase 

Type Property

# playUsingSceneTimeBase

Animations loaded from the scene file are immediately added to the scene and played according to the scene’s sceneTime property.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
static let playUsingSceneTimeBase: SCNSceneSource.AnimationImportPolicy
```

## Discussion

Using this policy is equivalent to manually loading each animation, setting its usesSceneTimeBase property to true, and adding it to the appropriate element of the scene. Use this policy when you want to directly control (or let the user directly control) the progress of animations.

## See Also

### Type Properties

static let doNotPlay: SCNSceneSource.AnimationImportPolicy

Animations are not loaded from the scene file.

static let play: SCNSceneSource.AnimationImportPolicy

Animations loaded from the scene file are immediately added to the scene and played once.

static let playRepeatedly: SCNSceneSource.AnimationImportPolicy

Animations loaded from the scene file are immediately added to the scene and played repeatedly.

