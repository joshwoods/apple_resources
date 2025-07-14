

- ARKit
- ARError
- ARError.Code
-  ARError.Code.geoTrackingFailed 

Case

# ARError.Code.geoTrackingFailed

An error that indicates when localization imagery fails to match the device’s camera captures.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case geoTrackingFailed
```

## Discussion

ARKit will raise an error with this error code when visual localization is taking too long. This situation indicates that the app has met all requirements for geo tracking except for visual localization. To try again, the app needs to ask the user pan the device around the physical environment to acquire different camera-feed imagery. For more information, see Assisting the User with Visual Localization.

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

