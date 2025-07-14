

- Swift Charts
- ChartProxy
-  value(at:as:) 

Instance Method

# value(at:as:)

Returns the data values at the given position, or `nil` if the position does not correspond to a valid Y value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func value(
    at position: CGPoint,
    as: (X, Y).Type = (X, Y).self
) -> (X, Y)? where X : Plottable, Y : Plottable
```

## Parameters 

`position`  

The position at which to obtain the data values. It should be relative to the plot.

## Return Value

A tuple of the x and y data values at the given position.

