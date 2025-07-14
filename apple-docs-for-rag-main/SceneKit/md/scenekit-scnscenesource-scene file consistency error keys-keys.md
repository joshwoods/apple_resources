

- SceneKit
- SCNSceneSource
-  Scene File Consistency Error Keys 

API Collection

# Scene File Consistency Error Keys

Keys identifying errors found during a scene-file-format consistency check.

## Overview

If you specify true for the checkConsistency when creating or loading from a scene source, SceneKit verifies the scene file against the specification for its file format. SceneKit reports any format verification issues that occur as an array of dictionaries, identified by the in the SCNDetailedErrorsKey key in the userInfo dictionary of an NSError object. Each item in the array is a dictionary containing one or more of the keys listed above.

These keys and their values provide details about the location of the error in the scene file. Other properties of the returned NSError object describe the nature of the validation error.

## Topics

### Constants

let SCNConsistencyElementIDErrorKey: String

The identifier of the scene file element where the error occurred.

let SCNConsistencyElementTypeErrorKey: String

The type of scene file element in which the error occurred.

let SCNConsistencyLineNumberErrorKey: String

The line number in the scene file in which the error occurred.

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

Scene Loading Error Keys

Scene File Consistency Check Error Codes

Error codes that identify errors found during a scene-file-format consistency check.

typealias SCNSceneSourceStatusHandler

The signature for the block that SceneKit calls periodically to report progress while loading a scene.

enum SCNSceneSourceStatus

Constants identifying phases of SceneKit’s scene loading process, used in a SCNSceneSourceStatusHandler block.

