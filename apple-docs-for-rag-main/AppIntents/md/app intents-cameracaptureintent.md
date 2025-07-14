

- App Intents
-  CameraCaptureIntent 

Protocol

# CameraCaptureIntent

Designates intent that will launch an activity that uses device’s camera to capture photos or videos. Marking your intent with this protocol makes it available as a possible action for Camera quick action.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
protocol CameraCaptureIntent : SystemIntent
```

## Topics

### Associated Types

associatedtype AppContext : Decodable, Encodable, Sendable = Never

Container type used for storing and retrieving app specific information that can be accessed whenever (and wherever) this intent gets run

**Required**

### Type Properties

static var appContext: Self.AppContext?

An app context that an app can use to pass necessary information to the sandboxed capture extension. The system will retrieve this app context when necessary and inject it for use during

### Type Methods

static func updateAppContext(Self.AppContext?) async throws

Whenever the in-app context for this intent changes any process containing this intent can call this method to provide updated state to the system.

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

