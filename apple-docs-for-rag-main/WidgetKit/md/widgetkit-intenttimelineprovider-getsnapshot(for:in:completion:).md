

- WidgetKit
- IntentTimelineProvider
-  getSnapshot(for:in:completion:) 

Instance Method

# getSnapshot(for:in:completion:)

Provides a timeline entry representing the current time and state of a widget.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
@preconcurrency
func getSnapshot(
    for configuration: Self.Intent,
    in context: Self.Context,
    completion: @escaping (Self.Entry) -> Void
)
```

**Required**

## Parameters 

`configuration`  

The intent containing user-customized values.

`context`  

An object describing the context to show the widget in.

`completion`  

The completion handler to call after you create the snapshot entry.

## Discussion

WidgetKit calls `getSnapshot(for:in:completion:)` when the widget appears in transient situations. If context.isPreview is true, the widget appears in the widget gallery. In that case, call the completion handler as quickly as possible, perhaps supplying sample data if it could take more than a few seconds to fetch or calculate the widget’s current state.

The `configuration` parameter provides user-customized values, as defined in your custom intent definition.

## See Also

### Generating Timelines

func getTimeline(for: Self.Intent, in: Self.Context, completion: (Timeline&lt;Self.Entry>) -> Void)

Provides an array of timeline entries for the current time and, optionally, any future times to update a widget.

**Required**

func placeholder(in: Self.Context) -> Self.Entry

Provides a timeline entry representing a placeholder version of the widget.

**Required**

associatedtype Entry : TimelineEntry

A type that specifies the date to display a widget, and, optionally, indicates the current relevance of the widget’s content.

**Required**

associatedtype Intent : INIntent

The intent that contains user-customized values.

**Required**

func recommendations() -> [IntentRecommendation&lt;Self.Intent>]

Returns a set of intent recommendations you use to offer pre-configured widgets on platforms that don’t offer a dedicated user interface for customizing widget intents.

**Required** Default implementation provided.

typealias Context

An object that contains details about how a widget is rendered, including its size and whether it appears in the widget gallery.

