

- ARKit
- ARError
- ARError.Code
-  ARError.Code.highResolutionFrameCaptureInProgress 

Case

# ARError.Code.highResolutionFrameCaptureInProgress

An error that indicates the system needs to finish a high-resolution frame request before accepting another request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
case highResolutionFrameCaptureInProgress
```

## Discussion

The system provides this error to the completion handler of captureHighResolutionFrame(completion:) for failed operations.

## See Also

### Errors

case requestFailed

An error that indicates a request fails.

case cameraUnauthorized

An error that indicates the app lacks user permission for the camera.

case fileIOFailed

An error that indicates a file access fails to read or write.

case insufficientFeatures

An error that indicates the framework requires more features to complete a task.

case invalidCollaborationData

An error that indicates the framework fails to parse collaboration data the app receives over the network.

case invalidConfiguration

An error that indicates the configuration contains ambiguous or erroneous data.

case invalidReferenceImage

An error that indicates the framework fails to process a reference image.

case invalidReferenceObject

An error that indicates the framework fails to process a reference object.

case invalidWorldMap

An error that indicates the framework fails to process a world map.

case microphoneUnauthorized

An error that indicates the app lacks user permission for the microphone.

case objectMergeFailed

An error that indicates the framework fails to merge a detected object.

case sensorFailed

An error that indicates a sensor fails to provide required input.

case sensorUnavailable

An error that indicates the framework fails to access a required sensor.

case unsupportedConfiguration

An error that indicates the device lacks support for the session’s configuration.

case worldTrackingFailed

An error that indicates when world tracking experiences an unrecoverable problem.

