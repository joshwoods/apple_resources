

- WidgetKit
-  TimelineProviderContext 

Structure

# TimelineProviderContext

An object that contains details about how a widget is rendered, including its size and whether it appears in the widget gallery.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
struct TimelineProviderContext
```

## Overview

When requesting timelines for a widget, WidgetKit passes the TimelineProvider a context object that includes details about how the widget appears. These details include:

- The WidgetFamily; for example, WidgetFamily.systemSmall and WidgetFamily.systemMedium.

- The size, in points, of the widget.

- Variants of the environments where the widget might appear.

- Whether the widget appears as a preview in the widget gallery.

If your widget uses assets that take time to generate or depend on the specific environment they’re rendered in, you can use the environment variants to generate those assets in advance. Some of the common environment properties to consider include:

- colorScheme, where you use different assets for light and dark schemes.

- displayScale, where your widget might appear in both @1x and @2x displays on macOS devices.

To be responsive when the environment changes, WidgetKit may render the widget’s view in advance. For example, WidgetKit renders both light and dark versions of the widget so that if the color scheme changes, the correct version is immediately available.

## Topics

### Preparing Preview Content

let isPreview: Bool

A Boolean value that indicates when the widget appears in the widget gallery.

### Accessing Size Attributes

let family: WidgetFamily

The user-configured family of the widget: small, medium, or large.

let displaySize: CGSize

The size, in points, of the widget.

### Accessing Environment Variations

let environmentVariants: TimelineProviderContext.EnvironmentVariants

All environment values that might be set when a widget appears.

struct EnvironmentVariants

A structure containing all varieties of environments where a widget could appear.

## See Also

### Timeline management

Keeping a widget up to date

Plan your widget’s timeline to show timely, relevant information using dynamic views, and update the timeline when things change.

protocol TimelineProvider

A type that advises WidgetKit when to update a widget’s display.

protocol IntentTimelineProvider

A type that advises WidgetKit when to update a user-configurable widget’s display.

protocol TimelineEntry

A type that specifies the date to display a widget, and, optionally, indicates the current relevance of the widget’s content.

struct Timeline

An object that specifies a date for WidgetKit to update a widget’s view.

class WidgetCenter

An object that contains a list of user-configured widgets and is used for reloading widget timelines.

protocol AppIntentTimelineProvider

A type that advises WidgetKit when to update a user-configurable widget’s display.

