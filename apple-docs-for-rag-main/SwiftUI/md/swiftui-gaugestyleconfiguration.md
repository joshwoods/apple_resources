

- SwiftUI
-  GaugeStyleConfiguration 

Structure

# GaugeStyleConfiguration

The properties of a gauge instance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
struct GaugeStyleConfiguration
```

## Topics

### Describing the purpose of the gauge

var label: GaugeStyleConfiguration.Label

A view that describes the purpose of the gauge.

struct Label

A type-erased label of a gauge, describing its purpose.

### Reporting the range

var minimumValueLabel: GaugeStyleConfiguration.MinimumValueLabel?

A view that describes the minimum of the range for the current value.

struct MinimumValueLabel

A type-erased value label of a gauge describing the minimum value.

var maximumValueLabel: GaugeStyleConfiguration.MaximumValueLabel?

A view that describes the maximum of the range for the current value.

struct MaximumValueLabel

A type-erased value label of a gauge describing the maximum value.

### Setting the value

var value: Double

The current value of the gauge.

var currentValueLabel: GaugeStyleConfiguration.CurrentValueLabel?

A view that describes the current value.

struct CurrentValueLabel

A type-erased value label of a gauge that contains the current value.

struct MarkedValueLabel

A type-erased label describing a specific value of a gauge.

## See Also

### Styling indicators

func gaugeStyle&lt;S>(S) -> some View

Sets the style for gauges within this view.

protocol GaugeStyle

Defines the implementation of all gauge instances within a view hierarchy.

func progressViewStyle&lt;S>(S) -> some View

Sets the style for progress views in this view.

protocol ProgressViewStyle

A type that applies standard interaction behavior to all progress views within a view hierarchy.

struct ProgressViewStyleConfiguration

The properties of a progress view instance.

