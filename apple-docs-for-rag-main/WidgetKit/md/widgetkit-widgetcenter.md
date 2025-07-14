

- WidgetKit
-  WidgetCenter 

Class

# WidgetCenter

An object that contains a list of user-configured widgets and is used for reloading widget timelines.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
class WidgetCenter
```

## Mentioned in 

Making network requests in a widget extension

## Overview

WidgetCenter provides information about user-configured widgets, such as their family. For widgets that use IntentConfiguration, you can retrieve the user-edited values.

### Getting Configured Widget Information

To get a list of user-configured widgets, use getCurrentConfigurations(_:). This property provides an array of WidgetInfo objects containing the following information:

```
struct WidgetInfo {
    public let configuration: INIntent?
    public let family: WidgetFamily
    public let kind: String
}
```

The `kind` string matches the parameter you use when creating the widget’s StaticConfiguration or IntentConfiguration. The `family` property matches one of the options specified in the supportedFamilies(_:) property of the widget’s configuration. If your widget is based on IntentConfiguration, the `configuration` property provides the custom intent containing the user-customized values for each individual widget.

### Requesting a Reload of Your Widget’s Timeline

Changes in your app’s state may affect a widget’s timeline. When this happens, you can tell WidgetKit to reload the timeline for either a specific kind of widget or all widgets. For example, your app might register for push notifications based on the widgets the user has configured. When your app receives a push notification that changes the state for one or more of your widgets, requesting a reload of their timelines updates their display.

If you only need to reload a certain kind of widget, you can request a reload for only that kind. For example, in response to a push notification about a change in a game’s status, you could request a reload for only the game status widgets:

```
WidgetCenter.shared.reloadTimelines(ofKind: "com.mygame.gamestatus")
```

To request a reload for all of your widgets:

```
WidgetCenter.shared.reloadAllTimelines()
```

## Topics

### Getting Widget Information

static let shared: WidgetCenter

The shared widget center.

func getCurrentConfigurations((Result&lt;[WidgetInfo], any Error>) -> Void)

Retrieves information about user-configured widgets.

struct UserInfoKey

An object that defines keys for accessing information in a user info dictionary.

### Reloading Widget Timelines

func reloadTimelines(ofKind: String)

Reloads the timelines for all widgets of a particular kind.

func reloadAllTimelines()

Reloads the timelines for all configured widgets belonging to the containing app.

### Reloading Recommended Preconfigured Widgets

func invalidateConfigurationRecommendations()

Invalidates and refreshes the preconfigured intent configurations for user-customizable widgets.

### Instance Methods

func currentConfigurations() async throws -> [WidgetInfo]

Retrieves information about user-configured widgets.

func invalidateRelevance(ofKind: String)

Mark the relevance for a kind as invalid.

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

protocol AppIntentTimelineProvider

A type that advises WidgetKit when to update a user-configurable widget’s display.

