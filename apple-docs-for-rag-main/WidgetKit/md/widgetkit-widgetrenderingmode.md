

- WidgetKit
-  WidgetRenderingMode 

Structure

# WidgetRenderingMode

Constants that indicate the rendering mode for a widget.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 9.0+

``` source
struct WidgetRenderingMode
```

## Mentioned in 

Migrating ClockKit complications to WidgetKit

## Overview

The system can modify the appearance of accessory family widgets. For example, it renders widgets on the Lock Screen on iPhone using the vibrant mode, while it renders widget-based complications in watchOS using either the fullColor or accented modes, depending on the watch face and the user’s settings.

You can read the rendering mode from the environment values using the `.widgetRenderingMode` key.

```
@Environment(\.widgetRenderingMode) var widgetRenderingMode
```

You can then customize your widget’s design based on the rendering mode.

## Topics

### Rendering modes

static let fullColor: WidgetRenderingMode

The system renders the widget in full color.

static let accented: WidgetRenderingMode

The system divides the widget’s view hierarchy into an accent group and a default group, applying a different color to each group.

static let vibrant: WidgetRenderingMode

The system desaturates the widget, making a monochrome version that it uses to create an adaptive, vibrant effect.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable

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

enum WidgetFamily

Values that define the widget’s size and shape.

struct WidgetAccentedRenderingMode

Constants that indicate the rendering mode for an `Image` in when displayed in a widget in accented mode.

