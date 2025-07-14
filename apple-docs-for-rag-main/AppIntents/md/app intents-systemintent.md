

- App Intents
-  SystemIntent 

Protocol

# SystemIntent

Designates intent types provided by App Intents.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol SystemIntent : AppIntent
```

## Relationships

### Inherits From

- AppIntent
- PersistentlyIdentifiable
- Sendable

### Inherited By

- AudioPlaybackIntent
- AudioRecordingIntent
- AudioStartingIntent
- CameraCaptureIntent
- DeleteIntent
- LiveActivityIntent
- LiveActivityStartingIntent
- OpenIntent
- PauseWorkoutIntent
- PlayVideoIntent
- PushToTalkTransmissionIntent
- ResumeWorkoutIntent
- ShowInAppSearchResultsIntent
- StartDiveIntent
- StartWorkoutIntent

### Conforming Types

- OpenURLIntent

## See Also

### Actions

protocol AppIntent

An interface for providing an app-specific capability that people invoke from system experiences like Siri and the Shortcuts app.

protocol AudioPlaybackIntent

An App Intent that plays, pauses, or otherwise modifies audio playback state when it executes.

protocol AudioRecordingIntent

An app intent that starts, stops or otherwise modifies audio recording state.

protocol AudioStartingIntent

An App Intent that plays, pauses, or otherwise modifies audio playback state when it executes.

Deprecated

protocol CameraCaptureIntent

Designates intent that will launch an activity that uses device’s camera to capture photos or videos. Marking your intent with this protocol makes it available as a possible action for Camera quick action.

protocol DeleteIntent

Delete the associated entity(s).

protocol DeprecatedAppIntent

An app intent that marks an action as deprecated and informs people which action to use instead.

protocol ForegroundContinuableIntent

A protocol you use for app intents which begin their work with the app in the background but may request to continue in the foreground.

protocol OpenIntent

Open the associated item.

struct OpenURLIntent

An intent that opens a universal link.

protocol PlayVideoIntent

An intent that looks for videos based on a search term, then plays the content.

protocol ProgressReportingIntent

An intent that reports progress to the system during its execution

protocol PushToTalkTransmissionIntent

An intent that begins or ends an audio transmission with the Push to Talk framework.

protocol URLRepresentableIntent

An app intent with a URL representation.

protocol SetValueIntent

An intent that contains a value which can be set.

