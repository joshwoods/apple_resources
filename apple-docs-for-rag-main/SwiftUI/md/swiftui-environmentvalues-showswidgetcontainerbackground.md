

- SwiftUI
- EnvironmentValues
-  showsWidgetContainerBackground 

Instance Property

# showsWidgetContainerBackground

An environment variable that indicates whether the background of a widget appears.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+watchOS 8.0+

``` source
var showsWidgetContainerBackground: Bool { get }
```

## Return Value

`true` if, by default, the background appears in this context; `false` otherwise.

## Discussion

In iOS 16 and earlier, this environment variable is always `true` for system widgets and `false` for accessory widgets. In macOS 13 and earlier, and in watchOS 9 and earlier, it always evaluates to `true`.

If you pass `false` to containerBackgroundRemovable(_:) to always show the widget background, the system shows the widget background even if `showsWidgetContainerBackground` evaluates to `true`.

## See Also

### Widgets

var showsWidgetLabel: Bool

A Boolean value that indicates whether an accessory family widget can display an accessory label.

var widgetFamily: WidgetFamily

The template of the widget — small, medium, or large.

var widgetRenderingMode: WidgetRenderingMode

The widget’s rendering mode, based on where the system is displaying it.

var widgetContentMargins: EdgeInsets

A property that identifies the content margins of a widget.

