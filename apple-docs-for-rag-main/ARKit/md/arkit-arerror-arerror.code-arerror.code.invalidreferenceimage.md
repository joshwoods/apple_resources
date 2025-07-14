

- ARKit
- ARError
- ARError.Code
-  ARError.Code.invalidReferenceImage 

Case

# ARError.Code.invalidReferenceImage

An error that indicates the framework fails to process a reference image.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
case invalidReferenceImage
```

## Discussion

This error occurs when you supply a reference image to the configuration’s detectionImages but ARKit determined it’s unusable. This can happen when the image data doesn’t contain enough features to identify a unique picture, for example, it’s all white.

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

case geoTrackingFailed

An error that indicates when localization imagery fails to match the device’s camera captures.

