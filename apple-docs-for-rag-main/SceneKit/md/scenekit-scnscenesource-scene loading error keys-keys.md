

- SceneKit
- SCNSceneSource
-  Scene Loading Error Keys 

API Collection

# Scene Loading Error Keys

## Discussion

Keys identifying errors returned when creating scene sources or loading the scenes they contain, used in the userInfo dictionary of NSError objects.

## Topics

### Constants

let SCNDetailedErrorsKey: String

Detailed error information from SceneKit’s scene file loading process.

## See Also

### Constants

struct LoadingOption

Options for creating scene sources and loading the scenes they contain.

Scene Source Properties

The metadata properties associated with a scene file, used by the property(forKey:) method.

Contributor Keys

Metadata identifying the user and authoring tool that created a scene file, used with the SCNSceneSourceAssetContributorsKey key.

Unit Dictionary Keys

Metadata describing the unit of measurement used in a scene file, used with the SCNSceneSourceAssetUnitKey key.

Scene File Consistency Error Keys

Keys identifying errors found during a scene-file-format consistency check.

Scene File Consistency Check Error Codes

Error codes that identify errors found during a scene-file-format consistency check.

typealias SCNSceneSourceStatusHandler

The signature for the block that SceneKit calls periodically to report progress while loading a scene.

enum SCNSceneSourceStatus

Constants identifying phases of SceneKit’s scene loading process, used in a SCNSceneSourceStatusHandler block.

