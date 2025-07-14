

- App Intents
-  ShowInAppSearchResultsIntent 

Protocol

# ShowInAppSearchResultsIntent

An app intent that takes a person to search results for a specified search term.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.0+watchOS 10.2+

``` source
protocol ShowInAppSearchResultsIntent : SystemIntent
```

## Mentioned in 

Making in-app search actions available to Siri and Apple Intelligence

## Overview

Provide a SearchCriteria to specify a search term for this intent. You can provide several `ShowInAppSearchResultsIntent` implementations where each intent conforms to a different search criteria.

## Topics

### Scoping the search

static var searchScopes: Self.Criteria.SearchScopes

Values that help the system understand the scope of an app intent that shows the results of a string-based search.

**Required** Default implementations provided.

enum StringSearchScope

Constants that help the system understand the in-app search functionality and its searchable content.

### Defining the search criteria

var criteria: Self.Criteria

**Required**

protocol SearchCriteria

struct StringSearchCriteria

A structure that represents a string-based search request.

associatedtype Criteria : SearchCriteria

**Required**

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

protocol PushToTalkTransmissionIntent

An intent that begins or ends an audio transmission with the Push to Talk framework.

protocol URLRepresentableIntent

An app intent with a URL representation.

protocol SetValueIntent

An intent that contains a value which can be set.

