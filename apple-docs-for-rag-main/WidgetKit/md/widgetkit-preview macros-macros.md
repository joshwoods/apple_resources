

- WidgetKit
-  Preview macros 

API Collection

# Preview macros

Use Swift macros to create widget previews in Xcode.

## Topics

### Providing a widget preview

macro Preview&lt;Widget, Provider>(String?, as: WidgetFamily, widget: () -> Widget, timelineProvider: () -> Provider)

Preview a widget with a static configuration, using the specified timeline provider.

macro Preview&lt;Widget, Provider>(String?, as: WidgetFamily, using: Provider.Intent, widget: () -> Widget, timelineProvider: () -> Provider)

Preview a widget with an app intent configuration, using the specified timeline provider.

macro Preview&lt;Widget, Provider>(String?, as: WidgetFamily, using: Provider.Intent, widget: () -> Widget, timelineProvider: () -> Provider)

Preview a widget with an intent configuration, using the specified timeline provider.

macro Preview&lt;Widget>(String?, as: WidgetFamily, widget: () -> Widget, timeline: () async -> [any TimelineEntry])

Preview a timeline-style widget.

### Generating a Live Activity preview

macro Preview&lt;Widget, Attributes>(String?, as: ActivityPreviewViewKind, using: Attributes, widget: () -> Widget, contentStates: () async -> [Attributes.ContentState])

Preview a widget with an activity configuration, using the specified attributes and content states.

### Generated structures

struct PreviewActivityBuilder

struct PreviewTimelineBuilder

## See Also

### Widget preview and debugging

Previewing widgets and Live Activities in Xcode

Use Xcode previews to iteratively develop, fine-tune, and troubleshoot widgets and Live Activities.

Debugging Widgets

Set environment variables in Xcode to control your widget’s configuration in the debugger.

struct WidgetPreviewContext

A specification for the context of a widget preview.

