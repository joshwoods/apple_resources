

- SwiftUI
- GaugeStyleConfiguration
-  GaugeStyleConfiguration.MarkedValueLabel 

Structure

# GaugeStyleConfiguration.MarkedValueLabel

A type-erased label describing a specific value of a gauge.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
struct MarkedValueLabel
```

## Relationships

### Conforms To

- View

## See Also

### Setting the value

var value: Double

The current value of the gauge.

var currentValueLabel: GaugeStyleConfiguration.CurrentValueLabel?

A view that describes the current value.

struct CurrentValueLabel

A type-erased value label of a gauge that contains the current value.

