

- Accessibility
- AXChartDescriptor
-  xAxis 

Instance Property

# xAxis

The axis descriptor for the chart’s x-axis.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var xAxis: any AXDataAxisDescriptor { get set }
```

## See Also

### Specifying the axes

var yAxis: AXNumericDataAxisDescriptor?

The axis descriptor for the chart’s y-axis.

var additionalAxes: [any AXDataAxisDescriptor]

The descriptors for additional categorical or numerical axes beyond the x-axis and y-axis.

protocol AXDataAxisDescriptor

The basic interface for a data axis in a chart.

