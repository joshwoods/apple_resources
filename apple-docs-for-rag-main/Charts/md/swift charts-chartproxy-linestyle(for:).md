

- Swift Charts
- ChartProxy
-  lineStyle(for:) 

Instance Method

# lineStyle(for:)

Returns the line style for the given data value. Returns `nil` if the line style scale is unavailable, or the value is invalid.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func lineStyle(for value: P) -> StrokeStyle? where P : Plottable
```

## Parameters 

`value`  

The data value.

## Return Value

The line style corresponding to the data value, or `nil` if the data value is incompatible with the chart.

