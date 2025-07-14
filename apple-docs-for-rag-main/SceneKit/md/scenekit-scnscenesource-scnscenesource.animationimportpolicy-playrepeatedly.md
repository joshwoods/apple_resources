

- SceneKit
- SCNSceneSource
- SCNSceneSource.AnimationImportPolicy
-  playRepeatedly 

Type Property

# playRepeatedly

Animations loaded from the scene file are immediately added to the scene and played repeatedly.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
static let playRepeatedly: SCNSceneSource.AnimationImportPolicy
```

## Discussion

Using this policy is equivalent to manually loading each animation, setting its repeatCount property to `INFINITY`, and adding it to the appropriate element of the scene.

## See Also

### Type Properties

static let doNotPlay: SCNSceneSource.AnimationImportPolicy

Animations are not loaded from the scene file.

static let play: SCNSceneSource.AnimationImportPolicy

Animations loaded from the scene file are immediately added to the scene and played once.

static let playUsingSceneTimeBase: SCNSceneSource.AnimationImportPolicy

Animations loaded from the scene file are immediately added to the scene and played according to the scene’s sceneTime property.

