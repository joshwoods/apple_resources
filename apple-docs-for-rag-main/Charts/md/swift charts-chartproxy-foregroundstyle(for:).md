

- Swift Charts
- ChartProxy
-  foregroundStyle(for:) 

Instance Method

# foregroundStyle(for:)

Returns the foreground style for the given data value. Returns `nil` if the foreground style scale is unavailable, or the value is invalid.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func foregroundStyle(for value: P) -> AnyShapeStyle? where P : Plottable
```

## Parameters 

`value`  

The data value.

## Return Value

The foreground style corresponding to the data value, or `nil` if the data value is incompatible with the chart.

