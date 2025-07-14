

- SceneKit
- SCNSceneSource
-  Scene Source Properties 

API Collection

# Scene Source Properties

The metadata properties associated with a scene file, used by the property(forKey:) method.

## Topics

### Constants

let SCNSceneSourceAssetContributorsKey: String

The file contributors.

let SCNSceneSourceAssetCreatedDateKey: String

let SCNSceneSourceAssetModifiedDateKey: String

let SCNSceneSourceAssetUpAxisKey: String

let SCNSceneSourceAssetUnitKey: String

## See Also

### Constants

struct LoadingOption

Options for creating scene sources and loading the scenes they contain.

Contributor Keys

Metadata identifying the user and authoring tool that created a scene file, used with the SCNSceneSourceAssetContributorsKey key.

Unit Dictionary Keys

Metadata describing the unit of measurement used in a scene file, used with the SCNSceneSourceAssetUnitKey key.

Scene Loading Error Keys

Scene File Consistency Error Keys

Keys identifying errors found during a scene-file-format consistency check.

Scene File Consistency Check Error Codes

Error codes that identify errors found during a scene-file-format consistency check.

typealias SCNSceneSourceStatusHandler

The signature for the block that SceneKit calls periodically to report progress while loading a scene.

enum SCNSceneSourceStatus

Constants identifying phases of SceneKit’s scene loading process, used in a SCNSceneSourceStatusHandler block.

