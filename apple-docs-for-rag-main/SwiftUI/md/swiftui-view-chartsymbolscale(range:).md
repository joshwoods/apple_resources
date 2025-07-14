

- SwiftUI
- View
-  chartSymbolScale(range:) 

Instance Method

# chartSymbolScale(range:)

Configures the symbol style scale for charts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func chartSymbolScale(range: [any ChartSymbolShape]) -> some View
```

Show all declarations

## Parameters 

`range`  

The range of symbols that correspond to the scale domain.

## See Also

### Symbol scales

func chartSymbolScale(_:)

Configures the symbol scale for charts.

func chartSymbolScale&lt;Domain>(domain: Domain) -> some View

Configures the symbol style scale for charts.

func chartSymbolScale(domain:range:)

Configures the symbol style scale for charts.

func chartSymbolScale&lt;Domain, S>(domain: Domain, mapping: (Domain.Element) -> S) -> some View

Configures the symbol scale for charts.

func chartSymbolScale&lt;DataValue, S>(mapping: (DataValue) -> S) -> some View

Configures the symbol scale for charts.

