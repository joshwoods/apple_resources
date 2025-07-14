

- SwiftUI
- EnvironmentValues
-  widgetRenderingMode 

Instance Property

# widgetRenderingMode

The widget’s rendering mode, based on where the system is displaying it.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 9.0+

``` source
var widgetRenderingMode: WidgetRenderingMode { get set }
```

## Discussion

You can read the rendering mode from the environment values using this key.

```
@Environment(\.widgetRenderingMode) var widgetRenderingMode
```

Then modify the widget’s appearance based on the mode.

```
var body: some View {
    ZStack {
       switch renderingMode {
        case .fullColor:
           Text("Full color")
        case .accented:
           ZStack {
               Circle(...)
               VStack {
                   Text("Accented")
                       .widgetAccentable()
                   Text("Normal")
               }
           }
        case .vibrant:
           Text("Full color")
        default:
           ...
        }
    }
}
```

## See Also

### Widgets

var showsWidgetContainerBackground: Bool

An environment variable that indicates whether the background of a widget appears.

var showsWidgetLabel: Bool

A Boolean value that indicates whether an accessory family widget can display an accessory label.

var widgetFamily: WidgetFamily

The template of the widget — small, medium, or large.

var widgetContentMargins: EdgeInsets

A property that identifies the content margins of a widget.

