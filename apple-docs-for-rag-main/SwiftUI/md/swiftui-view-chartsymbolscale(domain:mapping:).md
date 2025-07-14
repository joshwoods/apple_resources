

- SwiftUI
- View
-  chartSymbolScale(domain:mapping:) 

Instance Method

# chartSymbolScale(domain:mapping:)

Configures the symbol scale for charts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func chartSymbolScale(
    domain: Domain,
    mapping: @escaping (Domain.Element) -> S
) -> some View where Domain : Collection, S : ChartSymbolShape, Domain.Element : Plottable
```

## Parameters 

`domain`  

The possible data values plotted as symbol in the chart.

`mapping`  

Maps data categories to symbol shapes.

## See Also

### Symbol scales

func chartSymbolScale(_:)

Configures the symbol scale for charts.

func chartSymbolScale&lt;Domain>(domain: Domain) -> some View

Configures the symbol style scale for charts.

func chartSymbolScale(domain:range:)

Configures the symbol style scale for charts.

func chartSymbolScale&lt;DataValue, S>(mapping: (DataValue) -> S) -> some View

Configures the symbol scale for charts.

func chartSymbolScale(range:)

Configures the symbol style scale for charts.

