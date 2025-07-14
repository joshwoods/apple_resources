

- App Intents
- AssistantSchemas
-  AssistantSchemas.CameraEnum 

Protocol

# AssistantSchemas.CameraEnum

Assistant schema conformance for types you use for camera functionality.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol CameraEnum : AssistantSchemas.Model
```

## Mentioned in 

Making camera actions available to Siri and Apple Intelligence

## Topics

### Instance Properties

var captureDevice: some AssistantSchemas.Enum

The device or camera for capturing a photo or video.

var captureDuration: some AssistantSchemas.Enum

The capture duration for a photo or video.

var captureMode: some AssistantSchemas.Enum

The capture mode for taking a photo or video.

## Relationships

### Inherits From

- AssistantSchemas.Model

### Conforming Types

- AssistantSchema.EnumSchema
- AssistantSchemas.EnumSchema

## See Also

### Camera

Making camera actions available to Siri and Apple Intelligence

Create app intents and enumerations to integrate your app’s camera functionality with Siri and Apple Intelligence.

protocol CameraIntent

Assistant schema conformance for app intents that offer camera functionality.

