

- App Intents
-  OpenURLIntent 

Structure

# OpenURLIntent

An intent that opens a universal link.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct OpenURLIntent
```

## Overview

Return an `OpenURLIntent` as the IntentResult of another app intent’s perform() method or use place the intent on a button that appears on an interactive widget or Live Activity.

Note that you need to use a universal link for your URL representation, you can’t use a custom URL scheme. For more information about universal links, see Allowing apps and websites to link to your content.

## Topics

### Initializers

init()

Creates an app intent.

init(URL)

init(urlRepresentable: some URLRepresentableEnum) throws

init(urlRepresentable: some URLRepresentableEntity) async throws

### Instance Properties

var $url: IntentParameter&lt;URL>

var url: URL

### Type Aliases

typealias PerformResult

typealias SummaryContent

The type of parameter summary representing this intent.

### Type Properties

static var title: LocalizedStringResource

A short, localized, human-readable string that describes the app intent using a verb and a noun in title case.

static var urlRepresentation: OpenURLIntent.URLRepresentation

### Default Implementations

AppIntent Implementations

PersistentlyIdentifiable Implementations

URLRepresentableIntent Implementations

## Relationships

### Conforms To

- AppIntent
- PersistentlyIdentifiable
- Sendable
- SystemIntent
- URLRepresentableIntent

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

