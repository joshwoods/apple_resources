

- ARKit
- ARError
-  unsupportedConfiguration 

Type Property

# unsupportedConfiguration

An error that indicates the device lacks support for the session’s configuration.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
static var unsupportedConfiguration: ARError.Code { get }
```

## Discussion

Call isSupported on an ARConfiguration to ensure it’s supported before attempting to create and run it on the session with runWithConfiguration:.

## See Also

### Identifying an error cause

enum Code

Codes that identify errors in ARKit.

static var requestFailed: ARError.Code

An error that indicates a request fails.

static var cameraUnauthorized: ARError.Code

An error that indicates the app lacks user permission for the camera.

static var fileIOFailed: ARError.Code

An error that indicates a file access fails to read or write.

static var insufficientFeatures: ARError.Code

An error that indicates the framework requires more features to complete a task.

static var invalidCollaborationData: ARError.Code

An error that indicates the framework fails to parse collaboration data the app receives over the network.

static var invalidConfiguration: ARError.Code

An error that indicates the configuration contains ambiguous or erroneous data.

static var invalidReferenceImage: ARError.Code

An error that indicates the framework fails to process a reference image.

static var invalidReferenceObject: ARError.Code

An error that indicates the framework fails to process a reference object.

static var invalidWorldMap: ARError.Code

An error that indicates the framework fails to process a world map.

static var microphoneUnauthorized: ARError.Code

An error that indicates the app lacks user permission for the microphone.

static var objectMergeFailed: ARError.Code

An error that indicates the framework fails to merge a detected object.

static var sensorFailed: ARError.Code

An error that indicates a sensor fails to provide required input.

static var sensorUnavailable: ARError.Code

An error that indicates the framework fails to access a required sensor.

static var worldTrackingFailed: ARError.Code

An error that indicates when world tracking experiences an unrecoverable problem.

