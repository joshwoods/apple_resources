

- Swift Charts
- ChartProxy
-  plotAreaFrame 

Instance Property

# plotAreaFrame

An anchor to the frame of the chart’s plot.

iOS 16.0–17.0DeprecatediPadOS 16.0–17.0DeprecatedMac Catalyst 16.0–17.0DeprecatedmacOS 13.0–14.0DeprecatedtvOS 16.0–17.0DeprecatedvisionOS 1.0+watchOS 9.0–10.0Deprecated

``` source
var plotAreaFrame: Anchor { get }
```

## Discussion

The plot is the area between the x and y axes, not including the axes themselves. If the chart is scrollable, the plot frame includes both visible and invisible portions of the plot.

A chart must exist in the context of the chart proxy. You can convert the anchor to a frame using a `GeometryProxy`.

