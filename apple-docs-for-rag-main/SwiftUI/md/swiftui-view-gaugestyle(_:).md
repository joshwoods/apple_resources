

- SwiftUI
- View
-  gaugeStyle(\_:) 

Instance Method

# gaugeStyle(\_:)

Sets the style for gauges within this view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func gaugeStyle(_ style: S) -> some View where S : GaugeStyle
```

## See Also

### Indicating a value

struct Gauge

A view that shows a value within a range.

struct ProgressView

A view that shows the progress toward completion of a task.

func progressViewStyle&lt;S>(S) -> some View

Sets the style for progress views in this view.

struct DefaultDateProgressLabel

The default type of the current value label when used by a date-relative progress view.

