

- WidgetKit
-  AccessoryWidgetBackground 

Structure

# AccessoryWidgetBackground

An adaptive background view that provides a standard appearance based on the the widget’s environment.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
struct AccessoryWidgetBackground
```

## Mentioned in 

Preparing widgets for additional platforms, contexts, and appearances

Migrating ClockKit complications to WidgetKit

## Overview

Use this view to provide a standardized background for your accessory widgets. Place the view in a ZStack behind your widget’s content.

```
ZStack {
    AccessoryWidgetBackground()
    VStack {
        Text("MON")
            .font(.caption)
            .widgetAccented()
        Text("6")
            .font(.title)
    }
}
```

The system only displays this view inside a WidgetFamily.accessoryCircular, WidgetFamily.accessoryCorner, or WidgetFamily.accessoryRectangular widget. In any other context, the system displays an empty view instead.

## Topics

### Creating accessory widget backgrounds

init()

Creates an instance of an accessory widget background.

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Presentation

Creating views for widgets, Live Activities, and watch complications

Implement glanceable views with WidgetKit and SwiftUI.

Preparing widgets for additional platforms, contexts, and appearances

Create widgets that support additional platforms and adapt to their context.

SwiftUI views for widgets

Present your app’s content in widgets with SwiftUI views.

Introducing SwiftUI

SwiftUI is a modern way to declare user interfaces for any Apple platform. Create beautiful, dynamic apps faster than ever before.

struct WidgetLocation

Values that indicate different widget locations.

