

- ARKit
- ARError
- ARError.Code
-  ARError.Code.microphoneUnauthorized 

Case

# ARError.Code.microphoneUnauthorized

An error that indicates the app lacks user permission for the microphone.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
case microphoneUnauthorized
```

## Discussion

When this error occurs, the app needs to prompt the user to give permission to use the microphone in Settings.

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

case geoTrackingFailed

An error that indicates when localization imagery fails to match the device’s camera captures.

