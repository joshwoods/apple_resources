

- SceneKit
- SCNSceneSource
-  SCNSceneSource.AnimationImportPolicy 

Structure

# SCNSceneSource.AnimationImportPolicy

Options for playing animations loaded from a scene file, used with the animationImportPolicy key in options dictionaries.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AnimationImportPolicy
```

## Topics

### Type Properties

static let doNotPlay: SCNSceneSource.AnimationImportPolicy

Animations are not loaded from the scene file.

static let play: SCNSceneSource.AnimationImportPolicy

Animations loaded from the scene file are immediately added to the scene and played once.

static let playRepeatedly: SCNSceneSource.AnimationImportPolicy

Animations loaded from the scene file are immediately added to the scene and played repeatedly.

static let playUsingSceneTimeBase: SCNSceneSource.AnimationImportPolicy

Animations loaded from the scene file are immediately added to the scene and played according to the scene’s sceneTime property.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Type Properties

static let animationImportPolicy: SCNSceneSource.LoadingOption

An option for controlling the playback of animations in a scene file.

static let assetDirectoryURLs: SCNSceneSource.LoadingOption

Locations to use for resolving relative URLs to external resources.

static let checkConsistency: SCNSceneSource.LoadingOption

An option to validate scene files while loading.

static let convertToYUp: SCNSceneSource.LoadingOption

An option for whether to transform assets loaded from the scene file for use in a coordinate system where the y-axis points up.

static let convertUnitsToMeters: SCNSceneSource.LoadingOption

An option for whether to automatically scale the scene’s contents.

static let createNormalsIfAbsent: SCNSceneSource.LoadingOption

An option for automatically generating surface normals if they are absent when loading geometry.

static let flattenScene: SCNSceneSource.LoadingOption

An option for automatically merging portions of a scene graph during loading.

static let overrideAssetURLs: SCNSceneSource.LoadingOption

An option to attempt loading external resources using their URLs as specified in a scene file.

static let preserveOriginalTopology: SCNSceneSource.LoadingOption

static let strictConformance: SCNSceneSource.LoadingOption

An option to interpret scene files exactly as specified by the scene file format.

static let useSafeMode: SCNSceneSource.LoadingOption

An option to limit filesystem and network access for external resources referenced by a scene file.

Deprecated

