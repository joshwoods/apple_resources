

- Swift Charts
- ChartProxy
-  position(for:) 

Instance Method

# position(for:)

Returns the x and y positions as a `CGPoint` for the given data values, or `nil` if either the X or the y scale is unavailable or if any data value is invalid. The returned position is relative to the plot.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func position(for point: (x: X, y: Y)) -> CGPoint? where X : Plottable, Y : Plottable
```

## Parameters 

`point`  

A tuple of x and y data values.

## Return Value

The position corresponding to the data values.

