

- App Intents
- AssistantSchemas
-  AssistantSchemas.CameraIntent 

Protocol

# AssistantSchemas.CameraIntent

Assistant schema conformance for app intents that offer camera functionality.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol CameraIntent : AssistantSchemas.Model
```

## Mentioned in 

Making camera actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var openInCaptureMode: some AssistantSchemas.Intent

The app intent conforms to the schema for opening the app’s camera functionality, ready to capture a photo or video.

var setDevice: some AssistantSchemas.Intent

The app intent conforms to the schema for choosing a device to capture a photo.

var startCapture: some AssistantSchemas.Intent

The app intent conforms to the schema for starting the capture of a photo or video.

var stopCapture: some AssistantSchemas.Intent

The app intent conforms to the schema for stopping the capture of a photo or video.

var switchDevice: some AssistantSchemas.Intent

The app intent conforms to the schema for switching between cameras or devices.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.IntentSchema
- AssistantSchemas.IntentSchema

## See Also

### Camera

Making camera actions available to Siri and Apple Intelligence

Create app intents and enumerations to integrate your app’s camera functionality with Siri and Apple Intelligence.

protocol CameraEnum

Assistant schema conformance for types you use for camera functionality.

