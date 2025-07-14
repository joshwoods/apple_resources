

- WidgetKit
- TimelineProvider
-  Entry 

Associated Type

# Entry

A type that specifies the date to display a widget, and, optionally, indicates the current relevance of the widget’s content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
associatedtype Entry : TimelineEntry
```

**Required**

## See Also

### Generating Timelines

func getSnapshot(in: Self.Context, completion: (Self.Entry) -> Void)

Provides a timeline entry that represents the current time and state of a widget.

**Required**

func getTimeline(in: Self.Context, completion: (Timeline&lt;Self.Entry>) -> Void)

Provides an array of timeline entries for the current time and, optionally, any future times to update a widget.

**Required**

func placeholder(in: Self.Context) -> Self.Entry

Provides a timeline entry representing a placeholder version of the widget.

**Required**

typealias Context

An object that contains details about how a widget is rendered, including its size and whether it appears in the widget gallery.

