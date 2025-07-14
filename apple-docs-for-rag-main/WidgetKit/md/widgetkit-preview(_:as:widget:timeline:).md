

- WidgetKit
-  Preview(\_:as:widget:timeline:) 

Macro

# Preview(\_:as:widget:timeline:)

Preview a timeline-style widget.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+watchOS 10.0+

``` source
@freestanding(declaration)
macro Preview(
    _ name: String? = nil,
    as family: WidgetFamily,
    widget: @escaping () -> Widget,
    @PreviewTimelineBuilder timeline: @escaping @MainActor () async -> [any TimelineEntry]
) where Widget : Widget
```

## Parameters 

`name`  

An optional display name for the preview, which will appear in the canvas.

`family`  

The widget family to display.

`widget`  

A closure producing the widget to be previewed.

`timeline`  

A closure building the timeline of entries to be previewed.

## Mentioned in 

Previewing widgets and Live Activities in Xcode

## Overview

The preview will allow you to step through your timeline and test out the transitions between entries. (The dates of the entries will be ignored.)

Note

The timeline entries must be of the type expected by the widget. (This will be enforced at run-time.)

## See Also

### Providing a widget preview

macro Preview&lt;Widget, Provider>(String?, as: WidgetFamily, widget: () -> Widget, timelineProvider: () -> Provider)

Preview a widget with a static configuration, using the specified timeline provider.

macro Preview&lt;Widget, Provider>(String?, as: WidgetFamily, using: Provider.Intent, widget: () -> Widget, timelineProvider: () -> Provider)

Preview a widget with an app intent configuration, using the specified timeline provider.

macro Preview&lt;Widget, Provider>(String?, as: WidgetFamily, using: Provider.Intent, widget: () -> Widget, timelineProvider: () -> Provider)

Preview a widget with an intent configuration, using the specified timeline provider.

