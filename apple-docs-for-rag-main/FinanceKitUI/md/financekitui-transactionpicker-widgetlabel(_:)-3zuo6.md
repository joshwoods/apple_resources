

- FinanceKitUI
- TransactionPicker
-  widgetLabel(\_:) 

Instance Method

# widgetLabel(\_:)

Returns a localized text label that displays additional content outside the accessory family widget’s main SwiftUI view.

FinanceKitUISwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
func widgetLabel(_ labelKey: LocalizedStringKey) -> some View
```

## Parameters 

`labelKey`  

A label generated from a localized string.

## Discussion

To add a text label to an accessory family widget, call this method on the widget’s main SwiftUI view, and pass in a supported LocalizedStringKey. The system determines whether it can use the text label. If it can’t, it ignores the label. The system also sets the label’s size, placement, and style based on the clock face. For example, setting the font and rendering the text along a curve.

The following widget families support text accessory labels:

- The WidgetFamily.accessoryCorner widget-based complication can display a curved text label on the inside edge of the corner. Adding a label to an accessory corner complication causes the main SwiftUI view to shrink to make space for the label.

- The WidgetFamily.accessoryCircular widget can display a text label in watchOS; however, WidgetKit only renders the label along the bezel on the Infograph watch face (the top circular complication).

