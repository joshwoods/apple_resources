

- App Intents
-  PushToTalkTransmissionIntent 

Protocol

# PushToTalkTransmissionIntent

An intent that begins or ends an audio transmission with the Push to Talk framework.

iOS 17.4+iPadOS 17.4+visionOS 1.0+

``` source
protocol PushToTalkTransmissionIntent : SystemIntent
```

## Overview

Create an app intent that confirms to this protocol to manually start or end an audio transmission that uses the Push to Talk framework. For additional information about transmitting audio with the Push to Talk framework, see Push to Talk.

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

protocol URLRepresentableIntent

An app intent with a URL representation.

protocol SetValueIntent

An intent that contains a value which can be set.

protocol ShowInAppSearchResultsIntent

An app intent that takes a person to search results for a specified search term.

