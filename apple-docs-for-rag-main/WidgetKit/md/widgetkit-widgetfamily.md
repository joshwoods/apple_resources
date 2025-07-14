

- WidgetKit
-  WidgetFamily 

Enumeration

# WidgetFamily

Values that define the widget’s size and shape.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
@preconcurrency
enum WidgetFamily
```

## Overview

Widgets can support one or more sizes, giving users the flexibility to configure their widgets however they like. Each widget size provides a different amount of space for detail, so consider which sizes work best for the type of information the widget displays. For more information about designing widgets, see Widgets or Complications.

Note

The sizes of widgets may vary across devices. Your widget content should be flexible and avoid using fixed values.

You specify the sizes your widget supports using the supportedFamilies(_:) property modifier when defining your widget’s configuration.

```
struct GameStatusWidget: Widget {
    var body: some WidgetConfiguration {
        StaticConfiguration(
            kind: "com.mygame.game-status",
            provider: GameStatusProvider(),
            placeholder: GameStatusPlaceholderView()
        ) { entry in
            GameStatusView(entry.gameStatus)
        }
        .configurationDisplayName("Game Status")
        .description("Shows an overview of your game status")
        .supportedFamilies([.systemSmall, .systemMedium, .systemLarge])
    }
}
```

When WidgetKit needs to load a widget’s timeline, it calls the TimelineProvider class’s getTimeline(in:completion:) method. The system passes a TimelineProviderContext instance to the method’s `context` parameter. Use the context’s family property to determine the widget’s size and shape. For example, the WidgetFamily.systemSmall family represents a small, square widget on the Home Screen or Today View in iOS or iPadOS, while, in watchOS theWidgetFamily.accessoryCorner family appears as a widget-based complication in the corner of a watch face.

Use the WidgetFamily value to return the appropriate content given the widget’s size. For example, a WidgetFamily.systemSmall widget may focus on showing only the most critical data, such as a single image or a simple gauge, while a WidgetFamily.systemLarge widget can contain additional details, more-complex graphs, and even small blocks of text.

## Topics

### Accessing system families

case systemSmall

A small widget.

case systemMedium

A medium-sized widget.

case systemLarge

A large widget.

case systemExtraLarge

An extra-large widget.

### Accessing accessory families

case accessoryCircular

A circular widget.

case accessoryCorner

A widget-based complication in the corner of a watch face in watchOS.

case accessoryRectangular

A rectangular widget.

case accessoryInline

A flat widget that contains a single row of text and an optional image.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

struct StaticConfiguration

An object describing the content of a widget that has no user-configurable options.

struct WidgetRenderingMode

Constants that indicate the rendering mode for a widget.

struct WidgetAccentedRenderingMode

Constants that indicate the rendering mode for an `Image` in when displayed in a widget in accented mode.

