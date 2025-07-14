

- SwiftUI
-  ProgressViewStyleConfiguration 

Structure

# ProgressViewStyleConfiguration

The properties of a progress view instance.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct ProgressViewStyleConfiguration
```

## Topics

### Configuring the label

var label: ProgressViewStyleConfiguration.Label?

A view that describes the task represented by the progress view.

struct Label

A type-erased label describing the task represented by the progress view.

### Configuring the current value label

var currentValueLabel: ProgressViewStyleConfiguration.CurrentValueLabel?

A view that describes the current value of a progress view.

struct CurrentValueLabel

A type-erased label that describes the current value of a progress view.

### Configuring progress completion

let fractionCompleted: Double?

The completed fraction of the task represented by the progress view, from `0.0` (not yet started) to `1.0` (fully complete), or `nil` if the progress is indeterminate or relative to a date interval.

## See Also

### Styling indicators

func gaugeStyle&lt;S>(S) -> some View

Sets the style for gauges within this view.

protocol GaugeStyle

Defines the implementation of all gauge instances within a view hierarchy.

struct GaugeStyleConfiguration

The properties of a gauge instance.

func progressViewStyle&lt;S>(S) -> some View

Sets the style for progress views in this view.

protocol ProgressViewStyle

A type that applies standard interaction behavior to all progress views within a view hierarchy.

