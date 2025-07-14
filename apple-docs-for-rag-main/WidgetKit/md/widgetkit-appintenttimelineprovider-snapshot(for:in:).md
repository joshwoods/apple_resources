

- WidgetKit
- AppIntentTimelineProvider
-  snapshot(for:in:) 

Instance Method

# snapshot(for:in:)

Provides a timeline entry representing the current time and state of a widget.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+watchOS 10.0+

``` source
func snapshot(
    for configuration: Self.Intent,
    in context: Self.Context
) async -> Self.Entry
```

**Required**

## Parameters 

`configuration`  

The intent containing user-customized values.

`context`  

An object describing the context to show the widget in.

## Return Value

A timeline entry representing the current time and state of a widget

## Discussion

WidgetKit calls `snapshot(for:in:)` when the widget appears in transient situations. If context.isPreview is true, the widget appears in the widget gallery. In that case, return the `Entry` as quickly as possible, perhaps supplying sample data if it could take more than a few seconds to fetch or calculate the widget’s current state.

The `configuration` parameter provides user-customized values, as defined in your custom intent.

## See Also

### Generating timelines

func placeholder(in: Self.Context) -> Self.Entry

Provides a timeline entry representing a placeholder version of the widget.

**Required**

func recommendations() -> [AppIntentRecommendation&lt;Self.Intent>]

Returns a set of intent recommendations you use to offer pre-configured widgets on platforms that don’t offer a dedicated user interface for customizing widget intents.

**Required** Default implementation provided.

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

