

- SceneKit
- SCNSceneSource
- SCNSceneSource.LoadingOption
-  convertUnitsToMeters 

Type Property

# convertUnitsToMeters

An option for whether to automatically scale the scene’s contents.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.10+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
static let convertUnitsToMeters: SCNSceneSource.LoadingOption
```

## Discussion

The value for this key is an NSNumber object containing a floating-point value. The default value is `nil`, specifying no unit conversion.

SceneKit’s physics simulation works best when one unit in the scene’s coordinate space corresponds to one meter in the physics world. When you load elements from scene files, provide a value for this key specifying the number of meters (in the coordinate space of the loaded scene) for each unit in the scene coordinate space of the elements to be loaded.

For example, an artist might design a game character using a scale where one unit is a US foot. To load this model for use in SceneKit’s meter-based coordinate space, specify a value of `0.3048` for this key.

This option has no effect for assets compressed by Xcode. Instead, use Xcode itself to convert units when compressing the assets.

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

