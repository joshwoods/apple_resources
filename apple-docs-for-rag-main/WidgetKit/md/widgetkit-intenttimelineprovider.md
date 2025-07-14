

- WidgetKit
-  IntentTimelineProvider 

Protocol

# IntentTimelineProvider

A type that advises WidgetKit when to update a user-configurable widget’s display.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
protocol IntentTimelineProvider
```

## Overview

An Intent timeline provider performs the same function as TimelineProvider, but it also incorporates user-configured details into timeline entries.

For example, in a widget that displays the health status of a game character the user has chosen, the provider receives a custom intent specifying the character to display. In your Xcode project, you then define a custom SiriKit Intent Definition file. The intent definition can include the character’s details such as its name, avatar, strategic alliances, and so on.

Xcode generates the following INIntent custom intent:

```
public class SelectCharacterIntent: INIntent {
    @NSManaged public var characterName: String?
    @NSManaged public var avatar: String?
    @NSManaged public var alliances: [String]?
    @NSManaged public var healthLevel: NSNumber?
}
```

Because users can add multiple instances of a particular widget, your provider needs a way to differentiate which instance WidgetKit is asking about. When WidgetKit calls getSnapshot(for:in:completion:) or getTimeline(for:in:completion:), it passes an instance of your custom `INIntent`, configured with the user-selected details. The game widget provider accesses the properties of the intent and includes them in the TimelineEntry. WidgetKit then invokes the widget configuration’s content closure, passing the timeline entry to allow the views to access the user-configured properties. For example, the provider might implement a `TimelineEntry` with properties corresponding to those in the custom intent:

```
struct CharacterDetailEntry: TimelineEntry {
    var date: Date
    var name: String?
    var avatar: String?
    var alliances: [String]?
    var healthLevel: Double?
}
```

To generate a snapshot, the game widget provider initializes the character detail entry using the properties from the intent.

```
struct CharacterDetailProvider: IntentTimelineProvider {
    func getSnapshot(for configuration: SelectCharacterIntent, in context: Context, completion: @escaping (CharacterDetailEntry) -> Void) {
        let entry = CharacterDetailEntry(
            date: Date(),
            name: configuration.characterName,
            avatar: configuration.avatar,
            alliances: configuration.alliances,
            healthLevel: configuration.healthLevel?.doubleValue
        )
        completion(entry)
    }
}
```

## Topics

### Generating Timelines

func getSnapshot(for: Self.Intent, in: Self.Context, completion: (Self.Entry) -> Void)

Provides a timeline entry representing the current time and state of a widget.

**Required**

func getTimeline(for: Self.Intent, in: Self.Context, completion: (Timeline&lt;Self.Entry>) -> Void)

Provides an array of timeline entries for the current time and, optionally, any future times to update a widget.

**Required**

func placeholder(in: Self.Context) -> Self.Entry

Provides a timeline entry representing a placeholder version of the widget.

**Required**

associatedtype Entry : TimelineEntry

A type that specifies the date to display a widget, and, optionally, indicates the current relevance of the widget’s content.

**Required**

associatedtype Intent : INIntent

The intent that contains user-customized values.

**Required**

func recommendations() -> [IntentRecommendation&lt;Self.Intent>]

Returns a set of intent recommendations you use to offer pre-configured widgets on platforms that don’t offer a dedicated user interface for customizing widget intents.

**Required** Default implementation provided.

typealias Context

An object that contains details about how a widget is rendered, including its size and whether it appears in the widget gallery.

### Instance Methods

func relevance() async -> WidgetRelevance&lt;Self.Intent>

Provides an object containing attributes that describe when a specific widget could be relevant.

**Required** Default implementation provided.

## See Also

### Related Documentation

class INIntent

A request to fulfill in your app or Intents extension.

### Timeline management

Keeping a widget up to date

Plan your widget’s timeline to show timely, relevant information using dynamic views, and update the timeline when things change.

protocol TimelineProvider

A type that advises WidgetKit when to update a widget’s display.

struct TimelineProviderContext

An object that contains details about how a widget is rendered, including its size and whether it appears in the widget gallery.

protocol TimelineEntry

A type that specifies the date to display a widget, and, optionally, indicates the current relevance of the widget’s content.

struct Timeline

An object that specifies a date for WidgetKit to update a widget’s view.

class WidgetCenter

An object that contains a list of user-configured widgets and is used for reloading widget timelines.

protocol AppIntentTimelineProvider

A type that advises WidgetKit when to update a user-configurable widget’s display.

