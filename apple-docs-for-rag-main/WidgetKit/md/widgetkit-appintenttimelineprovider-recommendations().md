

- WidgetKit
- AppIntentTimelineProvider
-  recommendations() 

Instance Method

# recommendations()

Returns a set of intent recommendations you use to offer pre-configured widgets on platforms that don’t offer a dedicated user interface for customizing widget intents.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+watchOS 10.0+

``` source
func recommendations() -> [AppIntentRecommendation]
```

**Required** Default implementation provided.

## Mentioned in 

Migrating ClockKit complications to WidgetKit

Making a configurable widget

## Default Implementations

### AppIntentTimelineProvider Implementations

func recommendations() -> [AppIntentRecommendation&lt;Self.Intent>]

Returns a set of intent recommendations you use to offer pre-configured widgets on platforms that don’t offer a dedicated user interface for customizing widget intents.

## See Also

### Generating timelines

func placeholder(in: Self.Context) -> Self.Entry

Provides a timeline entry representing a placeholder version of the widget.

**Required**

func snapshot(for: Self.Intent, in: Self.Context) async -> Self.Entry

Provides a timeline entry representing the current time and state of a widget.

**Required**

func timeline(for: Self.Intent, in: Self.Context) async -> Timeline&lt;Self.Entry>

Provides an array of timeline entries for the current time and, optionally, any future times to update a widget.

**Required**

typealias Context

An object that contains details about how a widget is rendered, including its size and whether it appears in the widget gallery.

associatedtype Entry : TimelineEntry

A type that specifies the date to display a widget, and, optionally, indicates the current relevance of the widget’s content.

**Required**

associatedtype Intent : WidgetConfigurationIntent

The intent that contains user-customized values.

**Required**

