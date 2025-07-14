

- WidgetKit
-  StaticConfiguration 

Structure

# StaticConfiguration

An object describing the content of a widget that has no user-configurable options.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
struct StaticConfiguration where Content : View
```

## Mentioned in 

Increasing the visibility of widgets in Smart Stacks

## Overview

The following example shows the configuration for the leaderboard widget of the Emoji Rangers: Supporting Live Activities, interactivity, and animations sample code project.

```
struct LeaderboardWidget: Widget {

    public var body: some WidgetConfiguration {
        StaticConfiguration(kind: EmojiRanger.LeaderboardWidgetKind, provider: LeaderboardProvider()) { entry in
            LeaderboardWidgetEntryView(entry: entry)
        }
        .configurationDisplayName("Ranger Leaderboard")
        .description("See all the rangers.")
        .supportedFamilies(LeaderboardWidget.supportedFamilies)
    }
}
```

Every widget has a unique `kind`, a string that you choose. You use this string to identify your widget when reloading its timeline with WidgetCenter.

The timeline provider is an object that determines the timeline for refreshing your widget. Providing future dates for updating your widget allows the system to optimize the refresh process.

The content closure contains the SwiftUI views that WidgetKit needs to render the widget. When WidgetKit invokes the content closure, it passes a timeline entry created by the widget provider’s getSnapshot(in:completion:) or getTimeline(in:completion:) method.

Modifiers let you specify the families your widget supports, and the details shown when users add or edit their widgets.

## Topics

### Creating a widget configuration

init&lt;Provider>(kind: String, provider: Provider, content: (Provider.Entry) -> Content)

Creates a configuration for a widget, with no user-configurable options.

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

@MainActor @preconcurrency func supplementalActivityFamilies(_ families: [ActivityFamily]) -> some WidgetConfiguration 

Sets the sizes that a Live Activity supports.

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

### Widget creation

Creating a widget extension

Display your app’s content in a convenient, informative widget on various devices.

Supporting additional widget sizes

Offer widgets in additional contexts by adding support for various widget sizes.

Creating accessory widgets and watch complications

Support accessory widgets that appear on the Lock Screen and as complications on Apple Watch.

Migrating ClockKit complications to WidgetKit

Leverage WidgetKit’s API to create watchOS complications using SwiftUI.

Building Widgets Using WidgetKit and SwiftUI

Create widgets to show your app’s content on the Home screen, with custom intents for user-customizable settings.

Emoji Rangers: Supporting Live Activities, interactivity, and animations

Offer Live Activities, controls, animate data updates, and add interactivity to widgets.

Backyard Birds: Building an app with SwiftData and widgets

Create an app with persistent data, interactive widgets, and an all new in-app purchase experience.

Fruta: Building a Feature-Rich App with SwiftUI

Create a shared codebase to build a multiplatform app that offers widgets and an App Clip.

@MainActor @preconcurrency protocol Widget

The configuration and content of a widget to display on the Home screen or in Notification Center.

@MainActor @preconcurrency protocol WidgetBundle

A container used to expose multiple widgets from a single widget extension.

enum WidgetFamily

Values that define the widget’s size and shape.

struct WidgetRenderingMode

Constants that indicate the rendering mode for a widget.

struct WidgetAccentedRenderingMode

Constants that indicate the rendering mode for an `Image` in when displayed in a widget in accented mode.

