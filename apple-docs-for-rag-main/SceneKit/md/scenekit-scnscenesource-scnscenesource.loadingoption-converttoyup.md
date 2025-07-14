

- SceneKit
- SCNSceneSource
- SCNSceneSource.LoadingOption
-  convertToYUp 

Type Property

# convertToYUp

An option for whether to transform assets loaded from the scene file for use in a coordinate system where the y-axis points up.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.10+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
static let convertToYUp: SCNSceneSource.LoadingOption
```

## Discussion

The value for this key is an NSNumber object containing a Boolean value. The default value is false.

SceneKit’s physics simulation works best when the y-axis of scene coordinate space corresponds to the “up” direction of the physics world. Some external 3D authoring tools use coordinate systems where a different axis points up. Specify true for this key to automatically transform all scene elements loaded from the file based on the SCNSceneSourceAssetUpAxisKey value stored in the file.

This option has no effect for assets compressed by Xcode. Instead, use Xcode itself to transform coordinate spaces when compressing the assets.

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

