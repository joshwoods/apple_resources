

- WidgetKit
-  AppIntentConfiguration 

Structure

# AppIntentConfiguration

An object describing the content of a widget that uses a custom intent to provide user-configurable options.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
struct AppIntentConfiguration where Intent : WidgetConfigurationIntent, Content : View
```

## Mentioned in 

Increasing the visibility of widgets in Smart Stacks

## Overview

The following example shows the configuration for a game widget that displays details about a chosen character.

```
struct CharacterDetailWidget: Widget {
    var body: some WidgetConfiguration {
        AppIntentConfiguration(
            kind: "com.mygame.character-detail",
            intent: SelectCharacterIntent.self,
            provider: CharacterDetailProvider(),
        ) { entry in
            CharacterDetailView(entry: entry)
        }
        .supportedFamilies([.systemSmall, .systemMedium, .systemLarge])
    }
}
```

Every widget has a unique `kind`, a string that you choose. You use this string to identify your widget when reloading its timeline with WidgetCenter.

The `intent` is a custom App Intent containing user-editable parameters.

The timeline provider is an object that determines the timeline for refreshing your widget. Providing future dates for updating your widget allows the system to optimize the refresh process.

The content closure contains the SwiftUI views that WidgetKit needs to render the widget. When WidgetKit invokes the content closure, it passes a timeline entry created by the widget provider’s snapshot(for:in:) or timeline(for:in:) method.

Modifiers let you specify the families your widget supports, and the details shown when users add or edit their widgets.

## Topics

### Creating a widget configuration

init&lt;Provider>(kind: String, intent: Intent.Type, provider: Provider, content: (Provider.Entry) -> Content)

Creates a configuration for a widget by using a custom intent to provide user-configurable options.

@MainActor @preconcurrency var body: Self.Body { get }

The content and behavior of this widget.

### Setting the display name

@MainActor @preconcurrency func configurationDisplayName&lt;S>(_ displayName: S) -> some WidgetConfiguration where S : StringProtocol 

Sets the name shown for a widget when a user adds or edits it using the specified string.

@MainActor @preconcurrency func configurationDisplayName(_ displayName: Text) -> some WidgetConfiguration 

Sets the name shown for a widget when a user adds or edits it using the contents of a text view.

@MainActor @preconcurrency func configurationDisplayName(_ displayNameKey: LocalizedStringKey) -> some WidgetConfiguration 

Sets the localized name shown for a widget when a user adds or edits the widget.

### Setting the description

@MainActor @preconcurrency func description(_ description: Text) -> some WidgetConfiguration 

Sets the description shown for a widget when a user adds or edits it using the contents of a text view.

@MainActor @preconcurrency func description&lt;S>(_ description: S) -> some WidgetConfiguration where S : StringProtocol 

Sets the description shown for a widget when a user adds or edits it using the specified string.

@MainActor @preconcurrency func description(_ descriptionKey: LocalizedStringKey) -> some WidgetConfiguration 

Sets the localized description shown for a widget when a user adds or edits the widget.

### Setting the supported families

@MainActor @preconcurrency func supportedFamilies(_ families: [WidgetFamily]) -> some WidgetConfiguration 

Sets the sizes that a widget supports.

### Handling background network requests

nonisolated func backgroundTask&lt;D, R>(_ task: BackgroundTask&lt;D, R>, action: @escaping (D) async -> R) -> some WidgetConfiguration where D : Sendable, R : Sendable 

Runs the given action when the system provides a background task.

@MainActor @preconcurrency func onBackgroundURLSessionEvents(matching matchingBlock: ((String) -> Bool)? = nil, _ urlSessionEvent: @escaping (String, @escaping () -> Void) -> Void) -> some WidgetConfiguration 

Adds an action to perform when events related to a URL session identified by a closure are waiting to be processed.

@MainActor @preconcurrency func onBackgroundURLSessionEvents(matching matchingString: String, _ urlSessionEvent: @escaping (String, @escaping () -> Void) -> Void) -> some WidgetConfiguration 

Adds an action to perform when events related to a URL session with a matching identifier are waiting to be processed.

## Relationships

### Conforms To

- Sendable
- WidgetConfiguration

## See Also

### Configurable widgets

Making a configurable widget

Give people the option to customize their widgets by adding a custom app intent to your project.

Migrating widgets from SiriKit Intents to App Intents

Configure your widgets for backward compatibility.

struct WidgetInfo

A structure that contains information about user-configured widgets.

struct AppIntentRecommendation

An object that describes a recommended intent configuration for a user-customizable widget.

struct IntentConfiguration

An object describing the content of a widget that uses a custom intent definition to provide user-configurable options.

struct IntentRecommendation

An object that describes a recommended intent configuration for a user-customizable widget.

