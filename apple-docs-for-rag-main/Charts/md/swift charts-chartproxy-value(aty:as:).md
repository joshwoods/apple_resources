

- Swift Charts
- ChartProxy
-  value(atY:as:) 

Instance Method

# value(atY:as:)

Returns the data value at the given y position, or `nil` if the position does not correspond to a valid Y value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func value(
    atY position: CGFloat,
    as: P.Type = P.self
) -> P? where P : Plottable
```

## Parameters 

`position`  

The position at which to obtain the y data value. It should be relative to the plot.

## Return Value

The data value at the given position.

