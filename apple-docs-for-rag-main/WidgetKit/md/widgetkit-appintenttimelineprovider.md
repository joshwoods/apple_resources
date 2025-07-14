

- WidgetKit
-  AppIntentTimelineProvider 

Protocol

# AppIntentTimelineProvider

A type that advises WidgetKit when to update a user-configurable widget’s display.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+watchOS 10.0+

``` source
protocol AppIntentTimelineProvider
```

## Mentioned in 

Migrating ClockKit complications to WidgetKit

Making a configurable widget

## Overview

An App Intent timeline provider performs the same function as TimelineProvider, but it also incorporates user-configured details into timeline entries.

For example, in a widget that displays the health status of a game character the user has chosen, the provider receives a custom intent specifying the character to display. In your app code, you then define a custom App Intent. The intent can include the character’s details such as its name, avatar, strategic alliances, and so on.

```
struct CharacterConfiguration: WidgetConfigurationIntent {
    static var title: LocalizedStringResource = "Character"

    @Parameter(title: "Name")
    var name: String

    @Parameter(title: "Avatar", default: "Player 1")
    var avatar: String

    @Parameter(title: "Alliances", default: [])
    var alliances: [String]

    @Parameter(title: "Health", default: 100.0)
    var healthLevel: Double
}
```

Because users can add multiple instances of a particular widget, your provider needs a way to differentiate which instance WidgetKit is asking about. When WidgetKit calls snapshot(for:in:) or timeline(for:in:), it passes an instance of your configuration intent, configured with the user-selected details. The game widget provider accesses the properties of the intent and includes them in the TimelineEntry. WidgetKit then invokes the widget configuration’s content closure, passing the timeline entry to allow the views to access the user-configured properties. For example, the provider might implement a `TimelineEntry` with properties corresponding to those in the custom intent:

```
struct CharacterDetailEntry: TimelineEntry {
    var date: Date
    var name: String
    var avatar: String
    var alliances: [String]
    var healthLevel: Double
}
```

To generate a snapshot, the game widget provider initializes the character detail entry using the properties from the intent.

```
struct CharacterDetailProvider: AppIntentTimelineProvider {
    func snapshot(for configuration: CharacterConfiguration, in context: Context) async -> CharacterDetailEntry {
        return CharacterDetailEntry(
            date: Date(),
            name: configuration.characterName,
            avatar: configuration.avatar,
            alliances: configuration.alliances,
            healthLevel: configuration.healthLevel?.doubleValue
        )
    }
}
```

## Topics

### Generating timelines

func placeholder(in: Self.Context) -> Self.Entry

Provides a timeline entry representing a placeholder version of the widget.

**Required**

func recommendations() -> [AppIntentRecommendation&lt;Self.Intent>]

Returns a set of intent recommendations you use to offer pre-configured widgets on platforms that don’t offer a dedicated user interface for customizing widget intents.

**Required** Default implementation provided.

func snapshot(for: Self.Intent, in: Self.Context) async -> Self.Entry

Provides a timeline entry representing the current time and state of a widget.

**Required**

func timeline(for: Self.Intent, in: Self.Context) async -> Timeline&lt;Self.Entry>

Provides an array of timeline entries for the current time and, optionally, any future times to update a widget.

**Required**

typealias Context

An object that contains details about how a widget is rendered, including its size and whether it appears in the widget gallery.

associatedtype Entry : TimelineEntry

A type that specifies the date to display a widget, and, optionally, indicates the current relevance of the widget’s content.

**Required**

associatedtype Intent : WidgetConfigurationIntent

The intent that contains user-customized values.

**Required**

### Instance Methods

func relevance() async -> WidgetRelevance&lt;Self.Intent>

Provides an object containing attributes that describe when a specific widget could be relevant.

**Required** Default implementation provided.

## See Also

### Timeline management

Keeping a widget up to date

Plan your widget’s timeline to show timely, relevant information using dynamic views, and update the timeline when things change.

protocol TimelineProvider

A type that advises WidgetKit when to update a widget’s display.

protocol IntentTimelineProvider

A type that advises WidgetKit when to update a user-configurable widget’s display.

struct TimelineProviderContext

An object that contains details about how a widget is rendered, including its size and whether it appears in the widget gallery.

protocol TimelineEntry

A type that specifies the date to display a widget, and, optionally, indicates the current relevance of the widget’s content.

struct Timeline

An object that specifies a date for WidgetKit to update a widget’s view.

class WidgetCenter

An object that contains a list of user-configured widgets and is used for reloading widget timelines.

