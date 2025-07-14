

- SwiftUI
- View
-  progressViewStyle(\_:) 

Instance Method

# progressViewStyle(\_:)

Sets the style for progress views in this view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func progressViewStyle(_ style: S) -> some View where S : ProgressViewStyle
```

## Parameters 

`style`  

The progress view style to use for this view.

## Discussion

For example, the following code creates a progress view that uses the “circular” style:

```
ProgressView()
    .progressViewStyle(.circular)
```

## See Also

### Indicating a value

struct Gauge

A view that shows a value within a range.

func gaugeStyle&lt;S>(S) -> some View

Sets the style for gauges within this view.

struct ProgressView

A view that shows the progress toward completion of a task.

struct DefaultDateProgressLabel

The default type of the current value label when used by a date-relative progress view.

