

- WidgetKit
-  WidgetAccentedRenderingMode 

Structure

# WidgetAccentedRenderingMode

Constants that indicate the rendering mode for an `Image` in when displayed in a widget in accented mode.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
struct WidgetAccentedRenderingMode
```

## Topics

### Type Properties

static let accented: WidgetAccentedRenderingMode

Specifies that the `Image` should be included as part of the accented widget group.

static let accentedDesaturated: WidgetAccentedRenderingMode

Maps the luminance of the `Image` in to the alpha channel, replacing color channels with the color applied to the accent group.

static let desaturated: WidgetAccentedRenderingMode

Maps the luminance of the `Image` in to the alpha channel, replacing color channels with the color applied to the default group.

static let fullColor: WidgetAccentedRenderingMode

Specifies that the `Image` should be rendered at full color with no other color modifications. Only applies to iOS.

## Relationships

### Conforms To

- Equatable
- Hashable

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

struct WidgetRenderingMode

Constants that indicate the rendering mode for a widget.

