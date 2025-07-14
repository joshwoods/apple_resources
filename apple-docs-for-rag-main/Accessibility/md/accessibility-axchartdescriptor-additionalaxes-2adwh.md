

- Accessibility
- AXChartDescriptor
-  additionalAxes 

Instance Property

# additionalAxes

The descriptors for additional categorical or numerical axes beyond the x-axis and y-axis.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var additionalAxes: [any AXDataAxisDescriptor] { get set }
```

## See Also

### Specifying the axes

var xAxis: any AXDataAxisDescriptor

The axis descriptor for the chart’s x-axis.

var yAxis: AXNumericDataAxisDescriptor?

The axis descriptor for the chart’s y-axis.

protocol AXDataAxisDescriptor

The basic interface for a data axis in a chart.

