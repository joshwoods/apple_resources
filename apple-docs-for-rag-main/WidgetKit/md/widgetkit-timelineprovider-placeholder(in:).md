

- WidgetKit
- TimelineProvider
-  placeholder(in:) 

Instance Method

# placeholder(in:)

Provides a timeline entry representing a placeholder version of the widget.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
func placeholder(in context: Self.Context) -> Self.Entry
```

**Required**

## Parameters 

`context`  

An object that describes the context in which to show the widget.

## Return Value

A timeline entry that represents a placeholder version of the widget.

## Mentioned in 

Migrating ClockKit complications to WidgetKit

## Discussion

When WidgetKit displays your widget for the first time, it renders the widget’s view as a placeholder. A placeholder view displays a generic representation of your widget, giving the user a general idea of what the widget shows. WidgetKit calls `placeholder(in:)` to request an entry representing the widget’s placeholder configuration. For example, the game status widget would implement this method as follows:

```
struct GameStatusProvider: TimelineProvider {
    func placeholder(in context: Context) -> SimpleEntry {
       GameStatusEntry(date: Date(), gameStatus: "—")
    }
}
```

In addition, WidgetKit may render your widget as a placeholder if users choose to hide sensitive information on Apple Watch or the iPhone Lock Screen. To learn more about redacting sensitive data, see Creating a widget extension.

Important

`placeholder(in:)` is synchronous and returns a `TimelineEntry` immediately. Return from `placeholder(in:)` as quickly as possible.

## See Also

### Generating Timelines

func getSnapshot(in: Self.Context, completion: (Self.Entry) -> Void)

Provides a timeline entry that represents the current time and state of a widget.

**Required**

func getTimeline(in: Self.Context, completion: (Timeline&lt;Self.Entry>) -> Void)

Provides an array of timeline entries for the current time and, optionally, any future times to update a widget.

**Required**

associatedtype Entry : TimelineEntry

A type that specifies the date to display a widget, and, optionally, indicates the current relevance of the widget’s content.

**Required**

typealias Context

An object that contains details about how a widget is rendered, including its size and whether it appears in the widget gallery.

