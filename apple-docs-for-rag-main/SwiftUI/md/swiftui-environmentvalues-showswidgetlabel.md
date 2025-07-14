

- SwiftUI
- EnvironmentValues
-  showsWidgetLabel 

Instance Property

# showsWidgetLabel

A Boolean value that indicates whether an accessory family widget can display an accessory label.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+watchOS 9.0+

``` source
var showsWidgetLabel: Bool { get set }
```

## Discussion

Use this value to determine if you can provide additional content, or possibly move some of the widget’s content out of the main view and into the widget label.

```

@Environment(\.widgetFamily) var widgetFamily
@Environment(\.showsWidgetLabel) var showsWidgetLabel

var body: some View {
   switch widgetFamily {
   case .accessoryCircular:
       if showsWidgetLabel {
           Image("cat_full")
               .widgetLabel(label: Text("Cats"))
       }
       else {
           VStack {
               Image("cat_small")
               Text("Cats")
           }
       }
   }
}

```

This environment value is most useful when defining the appearance for the WidgetFamily.accessoryCircular widget family, because it’s value can change depending on where the widget appears. For example, if the widget is the top circular complication on the Infograph watch face, the value is `true`. Otherwise it is `false`. The environment variable is always `false` in iOS.

Other families always have the same value, regardless of where the widget appears. For the WidgetFamily.accessoryCorner widget family, the value is always `true`. For other families, it is `false`.

## See Also

### Widgets

var showsWidgetContainerBackground: Bool

An environment variable that indicates whether the background of a widget appears.

var widgetFamily: WidgetFamily

The template of the widget — small, medium, or large.

var widgetRenderingMode: WidgetRenderingMode

The widget’s rendering mode, based on where the system is displaying it.

var widgetContentMargins: EdgeInsets

A property that identifies the content margins of a widget.

