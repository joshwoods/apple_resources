

- ARKit
- ARError
- ARError.Code
-  ARError.Code.cameraUnauthorized 

Case

# ARError.Code.cameraUnauthorized

An error that indicates the app lacks user permission for the camera.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
case cameraUnauthorized
```

## Discussion

To use the device’s camera:

- Your app’s Info.plist file must provide a message for the NSCameraUsageDescription key. If this key is missing, any attempt to run an AR session fails with this error.

- When your app first attempts to run an AR session or otherwise use the camera, iOS automatically shows an alert with your camera usage description message, asking the user to grant camera permission to your app. If the user accepts this request, the session begins; otherwise the session fails with this error.

- If the user has previously denied camera permission for your app, all attempts to run an AR session or otherwise use the camera fail with this error. To grant camera permission, the user must explicitly enable your app in the iOS Settings app, under Privacy \> Camera.

## See Also

### Errors

case requestFailed

An error that indicates a request fails.

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

case geoTrackingFailed

An error that indicates when localization imagery fails to match the device’s camera captures.

