

- SceneKit
-  SCNSceneSourceStatusHandler 

Type Alias

# SCNSceneSourceStatusHandler

The signature for the block that SceneKit calls periodically to report progress while loading a scene.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias SCNSceneSourceStatusHandler = (Float, SCNSceneSourceStatus, (any Error)?, UnsafeMutablePointer) -> Void
```

## Discussion

You provide a block with this signature when using the scene(options:statusHandler:) method.

The block takes four parameters:

totalProgress  
A floating-point number between `0.0` and `1.0` indicating the overall progress of loading the scene. A value of `0.0` indicates that the loading process has just begun, and a value of `1.0` indicates that the process has completed.

status  
A constant identifying one of the distinct phases of SceneKit’s loading procedure. See SCNSceneSourceStatus for possible values.

error  
An error object describing any error that has occurred during scene loading, or `nil` if no errors has been encountered.

stopLoading  
A reference to a Boolean value. Set `*stop` to true within the block to abort further processing of the scene source’s contents.

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

enum SCNSceneSourceStatus

Constants identifying phases of SceneKit’s scene loading process, used in a SCNSceneSourceStatusHandler block.

