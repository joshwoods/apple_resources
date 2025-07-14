

- Swift Charts
- ChartProxy
-  positionRange(forY:) 

Instance Method

# positionRange(forY:)

Returns the range of y position for the given data value, or `nil` if the x scale is unavailable or if the value is invalid. The returned position range is relative to the plot.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func positionRange(forY value: P) -> ClosedRange? where P : Plottable
```

## Parameters 

`value`  

The data value.

## Return Value

The position range corresponding to the data value.

## Discussion

For a continuous data value, the returned range is a single point. For a categorical data value, the returned range is the range of positions that correspond to the given category.

