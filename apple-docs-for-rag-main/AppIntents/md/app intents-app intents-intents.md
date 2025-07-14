

- App Intents
-  App intents 

API Collection

# App intents

Define the custom actions your app exposes to the system, and incorporate support for existing SiriKit intents.

## Overview

Use app intents to express your app’s capabilities to the system. An app intent includes the code you need to perform an action, and expresses the data you require from the system. The system exposes your actions directly from the Shortcuts app and in system experiences like Siri.

To define an action, create a type that adopts the AppIntent protocol, or a related protocol that provides the specific behavior you need. Annotate any key properties with the `@Parameter` property wrapper to let the system know you need the associated information to perform the action.

For more information about features App Intents enables, see Making actions and content discoverable and widely available.

## Topics

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

protocol ShowInAppSearchResultsIntent

An app intent that takes a person to search results for a specified search term.

protocol SystemIntent

Designates intent types provided by App Intents.

### Controls, widgets, and Live Activities

protocol ControlConfigurationIntent

An interface for configuring a Control Center module.

protocol LiveActivityStartingIntent

An intent that starts, pauses, or otherwise modifies a Live Activity.

Deprecated

protocol LiveActivityIntent

An intent that starts, pauses, or otherwise modifies a Live Activity when it runs.

protocol WidgetConfigurationIntent

An interface for configuring a WidgetKit widget.

### Siri and Apple Intelligence

Integrating actions with Siri and Apple Intelligence

Create app intents, entities, and enumerations that conform to assistant schemas to tap into the enhanced action capabilities of Siri and Apple Intelligence.

App intent domains

Make your app’s actions and content available to Siri and Apple Intelligence with assistant schemas.

### SiriKit intent migration

protocol CustomIntentMigratedAppIntent

An interface for replacing a custom SiriKit intent that allows existing shortcuts and donations to continue working.

### Dependency management

class AppDependencyManager

An object that manages the registration and initialization of an app intent’s dependencies.

class AppDependency

A property wrapper that resolves a registered dependency at runtime.

### Supplementary content

protocol AppIntentsPackage

A type that describes app intent definitions that aren’t part of an app bundle and their dependencies.

struct IntentDescription

The human-readable description and metadata for an app intent.

struct IntentDialog

The text you want the system to display, or speak, when requesting a value, asking for disambiguation, or confirming an action.

struct IntentDeprecation

class IntentProjection

Projections for an app intent that returns non-optional values for parameters.

struct IntentSystemContext

Information that the system makes available to an app intent while it performs its action.

### Results

protocol IntentResult

A type that contains the result of performing an action, and includes optional information to deliver back to the initiator.

struct IntentResultContainer

An object that represents the output of a completed intent.

protocol OpensIntent

The result of performing an action that delivers an app intent back to the initiator of the action.

protocol ProvidesDialog

The result of performing an action that delivers a dialog back to the initiator of the action.

protocol ReturnsValue

The result of performing an action that delivers a value back to the initiator.

protocol ShowsSnippetView

The result of performing an action that delivers a view back to the initiator of the action.

protocol ResultsCollection

A protocol representing a collection of returned items with support for sectioning.

### Extensions

protocol AppIntentsExtension

An interface for managing an extension’s configuration.

## See Also

### Actions

Intent discovery

Donate your app’s intents to the system to help it identify trends and predict future behaviors.

App Shortcuts

Integrate your app’s intents and entities with the Shortcuts app, Siri, Spotlight, and the Action button on supported iPhone and Apple Watch models.

