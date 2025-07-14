

- SceneKit
-  SCNSceneSourceStatus 

Enumeration

# SCNSceneSourceStatus

Constants identifying phases of SceneKit’s scene loading process, used in a SCNSceneSourceStatusHandler block.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum SCNSceneSourceStatus
```

## Overview

Use the information provided by these constants to describe the scene loading process in your app’s user interface. Because this enumeration leaves room for more detailed progress reports, you should compare the `status` parameter of a SCNSceneSourceStatusHandler block against these values for ordering, not for equality, as in the following example handler:

```
SCNSceneSourceStatusHandler myHandler =
^(float totalProgress, SCNSceneSourceStatus status, NSError *error, BOOL *stop) {
    if (status >= SCNSceneSourceStatusProcessing && status 

## Topics

### Constants

case error

An error occurred when SceneKit attempted to load the scene.

case parsing

SceneKit has begun deserializing the source file.

case validating

SceneKit has begun validating the scene file’s format.

case processing

SceneKit has begun generating scene graph objects from the scene file’s contents.

case complete

SceneKit has successfully finished loading the scene file’s contents.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

Scene File Consistency Check Error Codes

Error codes that identify errors found during a scene-file-format consistency check.

typealias SCNSceneSourceStatusHandler

The signature for the block that SceneKit calls periodically to report progress while loading a scene.

