

- WidgetKit
- TimelineProvider
-  getTimeline(in:completion:) 

Instance Method

# getTimeline(in:completion:)

Provides an array of timeline entries for the current time and, optionally, any future times to update a widget.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
@preconcurrency
func getTimeline(
    in context: Self.Context,
    completion: @escaping (Timeline) -> Void
)
```

**Required**

## Parameters 

`context`  

An object describing the context to show the widget in.

`completion`  

The completion handler to call after you create the timeline.

## Mentioned in 

Migrating ClockKit complications to WidgetKit

Making network requests in a widget extension

## See Also

### Generating Timelines

func getSnapshot(in: Self.Context, completion: (Self.Entry) -> Void)

Provides a timeline entry that represents the current time and state of a widget.

**Required**

func placeholder(in: Self.Context) -> Self.Entry

Provides a timeline entry representing a placeholder version of the widget.

**Required**

associatedtype Entry : TimelineEntry

A type that specifies the date to display a widget, and, optionally, indicates the current relevance of the widget’s content.

**Required**

typealias Context

An object that contains details about how a widget is rendered, including its size and whether it appears in the widget gallery.

