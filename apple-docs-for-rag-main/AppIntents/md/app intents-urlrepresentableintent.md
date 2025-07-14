

- App Intents
-  URLRepresentableIntent 

Protocol

# URLRepresentableIntent

An app intent with a URL representation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol URLRepresentableIntent : AppIntent
```

## Overview

Add support for `URLRepresentableIntent` to your app intents to add a URL representation. This allows Siri and Shortcuts to treat the intent like a universal link to specific content, allowing actions to open the URL or to make it sharable.

Note that you need to use a universal link for your URL representation, you can’t use a custom URL scheme. For more information about universal links, see Allowing apps and websites to link to your content.

## Topics

### Type Aliases

typealias URLRepresentation

### Type Properties

static var urlRepresentation: Self.URLRepresentation

**Required** Default implementations provided.

## Relationships

### Inherits From

- AppIntent
- PersistentlyIdentifiable
- Sendable

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

protocol SetValueIntent

An intent that contains a value which can be set.

protocol ShowInAppSearchResultsIntent

An app intent that takes a person to search results for a specified search term.

