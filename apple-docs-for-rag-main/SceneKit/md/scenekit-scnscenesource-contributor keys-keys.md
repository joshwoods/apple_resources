

- SceneKit
- SCNSceneSource
-  Contributor Keys 

API Collection

# Contributor Keys

Metadata identifying the user and authoring tool that created a scene file, used with the SCNSceneSourceAssetContributorsKey key.

## Overview

Authoring tools that generate scene files may include metadata identifying the name and version of the authoring software and the name of the user who created the file. The values for these keys are NSString objects.

## Topics

### Constants

let SCNSceneSourceAssetAuthoringToolKey: String

The authoring tool that created the scene file.

let SCNSceneSourceAssetAuthorKey: String

The author of the scene file.

## See Also

### Constants

struct LoadingOption

Options for creating scene sources and loading the scenes they contain.

Scene Source Properties

The metadata properties associated with a scene file, used by the property(forKey:) method.

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

