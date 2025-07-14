

- ARKit
- ARError
-  geoTrackingFailed 

Type Property

# geoTrackingFailed

An error that indicates when localization imagery fails to match the device’s camera captures.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
static var geoTrackingFailed: ARError.Code { get }
```

## Discussion

ARKit will raise an error with this error code when visual localization is taking too long. This situation indicates that the app has met all requirements for geo tracking except for visual localization. To try again, the app needs to ask the user pan the device around the physical environment to acquire different camera-feed imagery. For more information, see Assisting the User with Visual Localization.

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

static var unsupportedConfiguration: ARError.Code

An error that indicates the device lacks support for the session’s configuration.

