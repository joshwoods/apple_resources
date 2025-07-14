

- ARKit
- ARError
-  geoTrackingNotAvailableAtLocation 

Type Property

# geoTrackingNotAvailableAtLocation

An error that indicates a location lacks geotracking support.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
static var geoTrackingNotAvailableAtLocation: ARError.Code { get }
```

## Discussion

This error code indicates that ARKit does not have the necessary localization imagery to support geo tracking at the user’s current location. See checkAvailability(completionHandler:) for more information.

If checkAvailability(completionHandler:) returns true and an app begins geo-tracking session, ARKit provides this state reason when the user has moved to an unsupported area.

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

