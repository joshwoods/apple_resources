

- WidgetKit
-  ActivityConfiguration 

Structure

# ActivityConfiguration

An object that describes the content of a Live Activity.

iOS 16.1+iPadOS 16.1+

``` source
@MainActor @preconcurrency
struct ActivityConfiguration where Attributes : ActivityAttributes
```

## Overview

To learn more about offering Live Activities for your app, see ActivityKit.

## Topics

### Creating a Live Activity configuration

struct ActivityViewContext

A structure that describes the view context for creating the views of a Live Activity.

init&lt;Content>(for: Attributes.Type, content: (ActivityViewContext&lt;Attributes>) -> Content, dynamicIsland: (ActivityViewContext&lt;Attributes>) -> DynamicIsland)

Creates a configuration object for a Live Activity.

## Relationships

### Conforms To

- Sendable
- WidgetConfiguration

## See Also

### Live Activities

struct DynamicIsland

The layout and configuration for a Live Activity that appears in the Dynamic Island.

let NSUserActivityTypeLiveActivity: String

A string that the system passes to the app on launch from a Live Activity that doesn’t provide a URL.

enum ActivityPreviewViewKind

Values that represent Live Activity presentations for use in Xcode previews.

enum ActivityFamily

A family that defines the Live Activity’s size.

