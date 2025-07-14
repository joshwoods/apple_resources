

- SwiftUI
- View
-  chartYScale(domain:range:type:) 

Instance Method

# chartYScale(domain:range:type:)

Configures the y scale for charts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func chartYScale(
    domain: Domain,
    range: Range,
    type: ScaleType? = nil
) -> some View where Domain : ScaleDomain, Range : PositionScaleRange
```

## Parameters 

`domain`  

The possible data values along the y axis in the chart. You can define the domain with a `ClosedRange` for number or `Date` values (e.g., `0 ... 500`), and with an array for categorical values (e.g., `["A", "B", "C"]`)

`range`  

The range of y positions that correspond to the scale domain. By default the range is determined by the dimension of the plot area. You can use `range: .plotDimension(startPadding:, endPadding:)` to add padding to the scale range.

`type`  

The scale type.

## See Also

### Axis scales

func chartXScale&lt;Domain, Range>(domain: Domain, range: Range, type: ScaleType?) -> some View

Configures the x scale for charts.

func chartXScale&lt;Domain>(domain: Domain, type: ScaleType?) -> some View

Configures the x scale for charts.

func chartXScale&lt;Range>(range: Range, type: ScaleType?) -> some View

Configures the x scale for charts.

func chartXScale(type: ScaleType?) -> some View

Configures the x scale for charts.

func chartYScale&lt;Domain>(domain: Domain, type: ScaleType?) -> some View

Configures the y scale for charts.

func chartYScale&lt;Range>(range: Range, type: ScaleType?) -> some View

Configures the y scale for charts.

func chartYScale(type: ScaleType?) -> some View

Configures the y scale for charts.

