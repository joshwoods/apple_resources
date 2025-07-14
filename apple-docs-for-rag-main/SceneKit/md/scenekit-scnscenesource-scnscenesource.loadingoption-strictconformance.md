

- SceneKit
- SCNSceneSource
- SCNSceneSource.LoadingOption
-  strictConformance 

Type Property

# strictConformance

An option to interpret scene files exactly as specified by the scene file format.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let strictConformance: SCNSceneSource.LoadingOption
```

## Discussion

The value for this key is an NSNumber object containing a Boolean value. The default value is false.

By default, SceneKit reads additional metadata present in a scene file when loading a scene so that its rendering the scene’s contents is as close as possible to the original intent of the scene file’s author. This information can include options that an artist may select using third-party 3D authoring tools or features of SceneKit not specified by the scene file format. If you set this option’s value to true, SceneKit ignores information that is not part of the scene file format’s specification.

## See Also

### Type Properties

static let animationImportPolicy: SCNSceneSource.LoadingOption

An option for controlling the playback of animations in a scene file.

struct AnimationImportPolicy

Options for playing animations loaded from a scene file, used with the animationImportPolicy key in options dictionaries.

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

static let useSafeMode: SCNSceneSource.LoadingOption

An option to limit filesystem and network access for external resources referenced by a scene file.

Deprecated

