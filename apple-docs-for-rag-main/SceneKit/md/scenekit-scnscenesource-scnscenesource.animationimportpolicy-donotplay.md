

- SceneKit
- SCNSceneSource
- SCNSceneSource.AnimationImportPolicy
-  doNotPlay 

Type Property

# doNotPlay

Animations are not loaded from the scene file.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
static let doNotPlay: SCNSceneSource.AnimationImportPolicy
```

## Discussion

To play animations stored in the scene file, load them manually using the entryWithIdentifier:withClass: method.

## See Also

### Type Properties

static let play: SCNSceneSource.AnimationImportPolicy

Animations loaded from the scene file are immediately added to the scene and played once.

static let playRepeatedly: SCNSceneSource.AnimationImportPolicy

Animations loaded from the scene file are immediately added to the scene and played repeatedly.

static let playUsingSceneTimeBase: SCNSceneSource.AnimationImportPolicy

Animations loaded from the scene file are immediately added to the scene and played according to the scene’s sceneTime property.

