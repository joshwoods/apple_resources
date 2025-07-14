

- SwiftUI
- View
-  chartSymbolScale(domain:) 

Instance Method

# chartSymbolScale(domain:)

Configures the symbol style scale for charts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func chartSymbolScale(domain: Domain) -> some View where Domain : ScaleDomain
```

## Parameters 

`domain`  

The possible data values plotted as symbols in the chart. You can define the domain with an array for categorical values (e.g., `["A", "B", "C"]`)

## See Also

### Symbol scales

func chartSymbolScale(_:)

Configures the symbol scale for charts.

func chartSymbolScale(domain:range:)

Configures the symbol style scale for charts.

func chartSymbolScale&lt;Domain, S>(domain: Domain, mapping: (Domain.Element) -> S) -> some View

Configures the symbol scale for charts.

func chartSymbolScale&lt;DataValue, S>(mapping: (DataValue) -> S) -> some View

Configures the symbol scale for charts.

func chartSymbolScale(range:)

Configures the symbol style scale for charts.

