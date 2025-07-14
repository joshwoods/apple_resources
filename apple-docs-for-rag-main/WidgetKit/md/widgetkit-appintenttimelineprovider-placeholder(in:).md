

- WidgetKit
- AppIntentTimelineProvider
-  placeholder(in:) 

Instance Method

# placeholder(in:)

Provides a timeline entry representing a placeholder version of the widget.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+watchOS 10.0+

``` source
func placeholder(in context: Self.Context) -> Self.Entry
```

**Required**

## Parameters 

`context`  

An object that describes the context in which to show the widget.

## Return Value

A timeline entry that represents a placeholder version of the widget.

## Discussion

When WidgetKit displays your widget for the first time, it renders the widget’s view as a placeholder. A placeholder view displays a generic representation of your widget, giving the user a general idea of what the widget shows. WidgetKit calls `placeholder(in:)` to request an entry representing the widget’s placeholder configuration. For example, the game status widget would implement this method as follows:

```
struct GameStatusProvider: TimelineProvider {
    func placeholder(in context: Context) -> SimpleEntry {
       GameStatusEntry(date: Date(), gameStatus: "—")
    }
}
```

In addition, WidgetKit may render your widget as a placeholder if user’s choose to hide sensitive information on Apple Watch or the iPhone Lock Screen. To learn more about redacting sensitive data, see Creating a widget extension.

Important

`placeholder(in:)` is synchronous and returns a `TimelineEntry` immediately. Return from `placeholder(in:)` as quickly as possible.

## See Also

### Generating timelines

func recommendations() -> [AppIntentRecommendation&lt;Self.Intent>]

Returns a set of intent recommendations you use to offer pre-configured widgets on platforms that don’t offer a dedicated user interface for customizing widget intents.

**Required** Default implementation provided.

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

