

- Swift Charts
- ChartProxy
-  position(forX:) 

Instance Method

# position(forX:)

Returns the x position for the given data value, or `nil` if the x scale is unavailable or if the data value is invalid. The returned position is relative to the plot.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func position(forX value: P) -> CGFloat? where P : Plottable
```

## Parameters 

`value`  

A data value.

## Return Value

The position corresponding to the data value.

