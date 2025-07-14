

- MetricKit
- MXCellularConditionMetric
-  histogrammedCellularConditionTime 

Instance Property

# histogrammedCellularConditionTime

An object representing the distribution of the different levels of connectivity to the cellular network.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var histogrammedCellularConditionTime: MXHistogram { get }
```

## Discussion

Each bucket in the histogram is the percentage of total app runtime spent at the represented connectivity level during the reporting period.

## See Also

### Viewing cellular connectivity metrics

class MXUnitSignalBars

A unit of measure for the number of bars of cellular network connectivity.

