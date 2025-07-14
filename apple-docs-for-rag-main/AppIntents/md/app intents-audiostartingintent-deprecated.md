

- App Intents
-  AudioStartingIntent Deprecated

Protocol

# AudioStartingIntent

An App Intent that plays, pauses, or otherwise modifies audio playback state when it executes.

iPadOS 16.0–17.0DeprecatedMac Catalyst 16.0–17.0DeprecatedmacOS 13.0–14.0DeprecatedtvOS 16.0–17.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.0–10.0DeprecatediOS 16.0–17.0Deprecated

``` source
protocol AudioStartingIntent : SystemIntent
```

Deprecated

Please use AudioPlaybackIntent instead.

## Overview

Adopt this protocol to indicate to the system that your App Intent plays audio. The system can then avoid dialogue or other experiences that might interrupt that audio.

## Relationships

### Inherits From

- AppIntent
- PersistentlyIdentifiable
- Sendable
- SystemIntent

## See Also

### Actions

protocol AppIntent

An interface for providing an app-specific capability that people invoke from system experiences like Siri and the Shortcuts app.

protocol AudioPlaybackIntent

An App Intent that plays, pauses, or otherwise modifies audio playback state when it executes.

protocol AudioRecordingIntent

An app intent that starts, stops or otherwise modifies audio recording state.

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

protocol ShowInAppSearchResultsIntent

An app intent that takes a person to search results for a specified search term.

