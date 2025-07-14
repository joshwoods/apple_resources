

- Swift Charts
- ChartProxy
-  symbol(for:) 

Instance Method

# symbol(for:)

Returns the symbol for the given data value. Returns `nil` if the symbol scale is unavailable, or the value is invalid.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func symbol(for value: P) -> AnyChartSymbolShape? where P : Plottable
```

## Parameters 

`value`  

The data value.

## Return Value

The symbol corresponding to the data value, or `nil` if the data value is incompatible with the chart.

