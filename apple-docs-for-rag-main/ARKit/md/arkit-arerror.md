

- ARKit
-  ARError 

Structure

# ARError

An error reported by ARKit.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
struct ARError
```

## Topics

### Inspecting error information

static var errorDomain: String

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

static var worldTrackingFailed: ARError.Code

An error that indicates when world tracking experiences an unrecoverable problem.

static var geoTrackingFailed: ARError.Code

An error that indicates when localization imagery fails to match the device’s camera captures.

static var geoTrackingNotAvailableAtLocation: ARError.Code

An error that indicates a location lacks geotracking support.

static var locationUnauthorized: ARError.Code

An error that indicates the app lacks user permission for the device’s current location.

static var highResolutionFrameCaptureFailed: ARError.Code

An error that indicates a problem in the system’s capture pipeline.

static var highResolutionFrameCaptureInProgress: ARError.Code

An error that indicates the system needs to finish a high-resolution frame request before accepting another request.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

enum Code

Codes that identify errors in ARKit.

