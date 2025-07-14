

- SwiftUI
-  WidgetConfiguration 

Protocol

# WidgetConfiguration

A type that describes a widget’s content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
protocol WidgetConfiguration
```

## Overview

A type conforming to this protocol inherits `@preconcurrency @MainActor` isolation from the protocol if the conformance is included in the type’s base declaration:

```
struct MyCustomType: Transition {
    // `@preconcurrency @MainActor` isolation by default
}
```

Isolation to the main actor is the default, but it’s not required. Declare the conformance in an extension to opt out of main actor isolation:

```
extension MyCustomType: Transition {
    // `nonisolated` by default
}
```

## Topics

### Implementing a widget

var body: Self.Body

The content and behavior of this widget.

**Required**

associatedtype Body : WidgetConfiguration

The type of widget configuration representing the body of this configuration.

**Required**

### Setting a name

func configurationDisplayName(_:)

Sets the name shown for a widget when a user adds or edits it using the contents of a text view.

### Setting a description

func description(_:)

Sets the description shown for a widget when a user adds or edits it using the contents of a text view.

### Setting the appearance

func supportedFamilies([WidgetFamily]) -> some WidgetConfiguration

Sets the sizes that a widget supports.

func contentMarginsDisabled() -> some WidgetConfiguration

Disable default content margins.

func disfavoredLocations([WidgetLocation], for: [WidgetFamily]) -> some WidgetConfiguration

Sets the disfavored locations for a widget.

func containerBackgroundRemovable(Bool) -> some WidgetConfiguration

A modifier that marks the background of a widget as removable.

### Managing background tasks

func backgroundTask&lt;D, R>(BackgroundTask&lt;D, R>, action: (D) async -> R) -> some WidgetConfiguration

Runs the given action when the system provides a background task.

func onBackgroundURLSessionEvents(matching:_:)

Adds an action to perform when events related to a URL session identified by a closure are waiting to be processed.

### Instance Methods

func promptsForUserConfiguration() -> some WidgetConfiguration

Specifies that a widget’s configuration UI should be automatically presented after the widget is added.

func supplementalActivityFamilies([ActivityFamily]) -> some WidgetConfiguration

Sets the sizes that a Live Activity supports.

## Relationships

### Conforming Types

- EmptyWidgetConfiguration
- LimitedAvailabilityConfiguration

## See Also

### Creating widgets

Building Widgets Using WidgetKit and SwiftUI

Create widgets to show your app’s content on the Home screen, with custom intents for user-customizable settings.

Creating a widget extension

Display your app’s content in a convenient, informative widget on various devices.

Keeping a widget up to date

Plan your widget’s timeline to show timely, relevant information using dynamic views, and update the timeline when things change.

Making a configurable widget

Give people the option to customize their widgets by adding a custom app intent to your project.

protocol Widget

The configuration and content of a widget to display on the Home screen or in Notification Center.

protocol WidgetBundle

A container used to expose multiple widgets from a single widget extension.

struct LimitedAvailabilityConfiguration

A type-erased widget configuration.

struct EmptyWidgetConfiguration

An empty widget configuration.

