

- FinanceKitUI
- TransactionPicker
-  widgetCurvesContent(\_:) 

Instance Method

# widgetCurvesContent(\_:)

Displays the widget’s content along a curve if the context allows it.

FinanceKitUISwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
func widgetCurvesContent(_ curvesContent: Bool = true) -> some View
```

## Parameters 

`curvesContent`  

A Boolean value that indicates whether the system curves the widget label’s content, if the context allows.

## Discussion

The system positions the widget’s content along a curve that follows the corner of the watch face when displaying a WidgetFamily.accessoryCorner complication. The widget must use a widgetLabel(_:) modifier, and the curving effect modifies only text, SF Symbols, and images.

When displaying an `.accessoryCorner` complication, the system places the widget label on the inside of the curve, and the widget’s content on the outside, as shown below.

```
var body: some View {
    Text("Hi")
        .widgetCurvesContent()
        .widgetLabel("World!")
}
```

The system can also curve text, SF symbols, and image content from a ViewThatFits view.

```
var body: some View {
    ViewThatFits {
        Text("Hello")
        Text("Hi")
    }
    .widgetCurvesContent()
    .widgetLabel("World!")
}
```

