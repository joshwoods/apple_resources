

- App Intents
- App intent domains
-  Making camera actions available to Siri and Apple Intelligence 

Article

# Making camera actions available to Siri and Apple Intelligence

Create app intents and enumerations to integrate your app’s camera functionality with Siri and Apple Intelligence.

## Overview

To integrate your app’s camera capabilities with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent and app enumeration implementation that Apple Intelligence needs. For example, if your app allows a person to take a photo or video, use the AssistantIntent(schema:) macro and provide the assistant schema that consists of the `.camera` domain and the startCapture schema:

```
@AssistantIntent(schema: .camera.startCapture)
struct StartCaptureIntent {
    var captureMode: CaptureMode
    var timerDuration: CaptureDuration?
    var device: CaptureDevice?

    func perform() async throws -> some IntentResult {
        .result()
    }
}
```

To learn more about assistant schemas, see Integrating actions with Siri and Apple Intelligence. For a list of available app intents in the `.camera` domain, see AssistantSchemas.CameraIntent.

### Make sure your enumeration meets requirements

To make sure Siri and Apple Intelligence understand custom static types for your intent parameters, annotate app enumerations with the AssistantEnum(schema:) macro. Then, pass the `.camera` domain and a schema to it. The following example uses the captureMode schema:

```
@AssistantEnum(schema: .camera.captureMode)
struct CameraCaptureMode: String, AppEnum {
    // Your app's camera capture modes.
    case portrait
    case landscape
    case catFace
    case awesomeFilter

    static var caseDisplayRepresentations: [ClearHistoryTimeFrame: DisplayRepresentation] = [:]

}
```

For a list of available app enumeration schemas in the `.camera` domain, see AssistantSchemas.CameraEnum.

## See Also

### Camera

protocol CameraIntent

Assistant schema conformance for app intents that offer camera functionality.

protocol CameraEnum

Assistant schema conformance for types you use for camera functionality.

