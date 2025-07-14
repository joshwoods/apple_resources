

- SwiftUI
- WidgetConfiguration
-  contentMarginsDisabled() 

Instance Method

# contentMarginsDisabled()

Disable default content margins.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
func contentMarginsDisabled() -> some WidgetConfiguration
```

## Return Value

A modified widget configuration that doesn’t use default content margins.

## Discussion

When you disable content margins for a widget, the system doesn’t automatically add margins around the widget’s content, and you are responsible for specifying margins and padding around your widget content for each context. To specify custom margins, use widgetContentMargins in combination with doc://com.apple.documentation/swiftui/View/padding(\_) to selectively or partially apply the default content margins.

This modifier has no effect on operation system versions prior to iOS 17, watchOS 10, or macOS 14.

## See Also

### Setting the appearance

func supportedFamilies([WidgetFamily]) -> some WidgetConfiguration

Sets the sizes that a widget supports.

func disfavoredLocations([WidgetLocation], for: [WidgetFamily]) -> some WidgetConfiguration

Sets the disfavored locations for a widget.

func containerBackgroundRemovable(Bool) -> some WidgetConfiguration

A modifier that marks the background of a widget as removable.

