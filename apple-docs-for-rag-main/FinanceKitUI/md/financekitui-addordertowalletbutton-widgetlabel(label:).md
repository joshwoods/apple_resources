

- FinanceKitUI
- AddOrderToWalletButton
-  widgetLabel(label:) 

Instance Method

# widgetLabel(label:)

Creates a label for displaying additional content outside an accessory family widget’s main SwiftUI view.

FinanceKitUISwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
func widgetLabel(@ViewBuilder label: () -> Label) -> some View where Label : View
```

## Parameters 

`label`  

A view that WidgetKit can display alongside the accessory family widget’s main SwiftUI view. You can use a Image, Text, Gauge, ProgressView, or a container with multiple subviews.

## Discussion

The system only displays labels on widget-based complications in watchOS. The system ignores any labels attached to widgets on the Lock Screen on iPhone. Therefore, you can use the same code to display an accessory family widget on both iPhone and Apple Watch.

To create the widget label, call `widgetLabel(label:)`on a complication’s main SwiftUI view. Pass the desired content as the `label` parameter. The label can be a Gauge, ProgressView, Text, or Image. To provide multiple views, wrap your views in a container, such as a VStack. WidgetKit determines whether it can use any of the label’s content. If it can’t, it ignores the label.

```

  struct Complication: View {
      @Environment(\.widgetFamily) var widgetFamily

      var body: some View {
          switch widgetFamily {
          case .accessoryCorner:
              Text("Hi")
                  .widgetLabel {
                      Gauge(value: 0.8)
                  }
          case .accessoryCircular:
              VStack {
                  Image(systemName: "emoji.globe")
                  Text("Hi")
              }
              .widgetLabel("World!")
          case .accessoryInline:
              Text("\(Image(systemName: "emoji.globe.face")) World!")
      }
  }

```

WidgetKit configures the label so that the watch face presents a unified look. For example, it sets the size for an image, the font for text, and can even render text and gauges along a curve.

The following widget families support widget labels:

WidgetFamily.accessoryCorner  
In watchOS, this widget-based complication can display a Gauge, a ProgressView, or a Text. Adding a label to an accessory corner causes the main SwiftUI view to shrink to make space for the label. If you pass a view containing multiple, valid subviews, the system picks which view to display as the widget label.

WidgetFamily.accessoryCircular  
In watchOS, the widget-based complication can display either an Image or a Text. To pass both an image and text, wrap those views in a container.

However, WidgetKit only renders the label along the bezel on the Infograph watch face (the top circular complication). On all other circular complications — including widgets on all other platforms — WidgetKit ignores the label.

