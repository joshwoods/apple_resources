

- SwiftUI
- EnvironmentValues
-  widgetContentMargins 

Instance Property

# widgetContentMargins

A property that identifies the content margins of a widget.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+watchOS 10.0+

``` source
var widgetContentMargins: EdgeInsets { get }
```

## Return Value

Returns the content margins for the current widget presentation context.

## Discussion

The content margins of a widget depend on the context in which it appears. The system applies default content margins. However, if you disable automatic application of default content margins with contentMarginsDisabled(), the system uses the `widgetContentMargins` property in combination with padding(_:) to selectively apply default content margins.

## See Also

### Widgets

var showsWidgetContainerBackground: Bool

An environment variable that indicates whether the background of a widget appears.

var showsWidgetLabel: Bool

A Boolean value that indicates whether an accessory family widget can display an accessory label.

var widgetFamily: WidgetFamily

The template of the widget — small, medium, or large.

var widgetRenderingMode: WidgetRenderingMode

The widget’s rendering mode, based on where the system is displaying it.

