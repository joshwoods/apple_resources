

- SwiftUI
- View
-  complicationForeground() Deprecated

Instance Method

# complicationForeground()

Promotes this view to the foreground in a complication.

ClockKitSwiftUIwatchOS 7.0–11.4Deprecated

``` source
@MainActor @preconcurrency
func complicationForeground() -> some View
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Return Value

A view that is in the complication foreground.

## Discussion

A view in the foreground will be tinted alongside other foreground views. The color for both the foreground and background layers is determined by the watch face.

## See Also

### Appearance modifiers

func colorScheme(ColorScheme) -> some View

Sets this view’s color scheme.

Deprecated

func listRowPlatterColor(Color?) -> some View

Sets the color that the system applies to the row background when this view is placed in a list.

Deprecated

func background&lt;Background>(Background, alignment: Alignment) -> some View

Layers the given view behind this view.

Deprecated

func overlay&lt;Overlay>(Overlay, alignment: Alignment) -> some View

Layers a secondary view in front of this view.

Deprecated

func foregroundColor(Color?) -> some View

Sets the color of the foreground elements displayed by this view.

Deprecated

