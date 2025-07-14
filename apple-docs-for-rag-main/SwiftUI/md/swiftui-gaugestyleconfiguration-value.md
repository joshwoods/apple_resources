

- SwiftUI
- GaugeStyleConfiguration
-  value 

Instance Property

# value

The current value of the gauge.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
var value: Double
```

## Discussion

The valid range is `0.0...1.0`.

## See Also

### Setting the value

var currentValueLabel: GaugeStyleConfiguration.CurrentValueLabel?

A view that describes the current value.

struct CurrentValueLabel

A type-erased value label of a gauge that contains the current value.

struct MarkedValueLabel

A type-erased label describing a specific value of a gauge.

