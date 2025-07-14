

- Swift Charts
- ChartProxy
-  positionRange(for:) 

Instance Method

# positionRange(for:)

Returns the range of x and y positions for the given pair of data values, or `nil` if the y scale is unavailable or if the value is invalid.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func positionRange(for point: (x: X, y: Y)) -> CGRect? where X : Plottable, Y : Plottable
```

## Return Value

The position range corresponding to the data values.

## Discussion

For a continuous data value, the returned range is a single point. For a categorical data value, the returned range is the range of positions that correspond to the given category.

