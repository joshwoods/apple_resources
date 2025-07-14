

- WidgetKit
- TimelineProvider
-  getSnapshot(in:completion:) 

Instance Method

# getSnapshot(in:completion:)

Provides a timeline entry that represents the current time and state of a widget.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
@preconcurrency
func getSnapshot(
    in context: Self.Context,
    completion: @escaping (Self.Entry) -> Void
)
```

**Required**

## Parameters 

`context`  

An object describing the context to show the widget in.

`completion`  

The completion handler to call after you create the snapshot entry.

## Mentioned in 

Migrating ClockKit complications to WidgetKit

## Discussion

WidgetKit calls `getSnapshot(in:completion:)` when the widget appears in transient situations. If `context.isPreview` is `true`, the widget appears in the widget gallery. In that case, call the `completion` handler as quickly as possible, perhaps supplying sample data if it could take more than a few seconds to fetch or calculate the widget’s current state.

## See Also

### Generating Timelines

func getTimeline(in: Self.Context, completion: (Timeline&lt;Self.Entry>) -> Void)

Provides an array of timeline entries for the current time and, optionally, any future times to update a widget.

**Required**

func placeholder(in: Self.Context) -> Self.Entry

Provides a timeline entry representing a placeholder version of the widget.

**Required**

associatedtype Entry : TimelineEntry

A type that specifies the date to display a widget, and, optionally, indicates the current relevance of the widget’s content.

**Required**

typealias Context

An object that contains details about how a widget is rendered, including its size and whether it appears in the widget gallery.

