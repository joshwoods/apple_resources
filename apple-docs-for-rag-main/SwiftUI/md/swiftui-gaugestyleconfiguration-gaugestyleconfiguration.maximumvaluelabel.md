

- SwiftUI
- GaugeStyleConfiguration
-  GaugeStyleConfiguration.MaximumValueLabel 

Structure

# GaugeStyleConfiguration.MaximumValueLabel

A type-erased value label of a gauge describing the maximum value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
struct MaximumValueLabel
```

## Relationships

### Conforms To

- View

## See Also

### Reporting the range

var minimumValueLabel: GaugeStyleConfiguration.MinimumValueLabel?

A view that describes the minimum of the range for the current value.

struct MinimumValueLabel

A type-erased value label of a gauge describing the minimum value.

var maximumValueLabel: GaugeStyleConfiguration.MaximumValueLabel?

A view that describes the maximum of the range for the current value.

