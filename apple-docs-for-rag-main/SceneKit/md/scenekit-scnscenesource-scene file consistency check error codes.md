

- SceneKit
- SCNSceneSource
-  Scene File Consistency Check Error Codes 

API Collection

# Scene File Consistency Check Error Codes

Error codes that identify errors found during a scene-file-format consistency check.

## Overview

If you specify true for the checkConsistency when creating or loading from a scene source, SceneKit verifies the scene file against the specification for its file format. SceneKit reports any format verification issues in an NSError object whose code property is one of these values.

For more details about the location and nature of any format validation errors, see the SCNDetailedErrorsKey key in the error’s userInfo dictionary, and the keys listed in Scene File Consistency Error Keys.

## Topics

### Constants

var SCNConsistencyInvalidURIError: Int

The scene file contains an invalid URI (or URL).

var SCNConsistencyInvalidCountError: Int

The scene file contains an invalid number of scenes.

var SCNConsistencyInvalidArgumentError: Int

An element in the scene file contains an invalid option for one of its attributes.

var SCNConsistencyMissingElementError: Int

A required element in the scene file is missing.

var SCNConsistencyMissingAttributeError: Int

An element in the scene file is missing a required attribute.

var SCNConsistencyXMLSchemaValidationError: Int

The format of the scene file does not match its XML schema definition.

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

Scene File Consistency Error Keys

Keys identifying errors found during a scene-file-format consistency check.

typealias SCNSceneSourceStatusHandler

The signature for the block that SceneKit calls periodically to report progress while loading a scene.

enum SCNSceneSourceStatus

Constants identifying phases of SceneKit’s scene loading process, used in a SCNSceneSourceStatusHandler block.

