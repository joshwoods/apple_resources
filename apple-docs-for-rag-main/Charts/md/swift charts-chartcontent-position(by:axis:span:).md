

- Swift Charts
- ChartContent
-  position(by:axis:span:) 

Instance Method

# position(by:axis:span:)

Represents data using position.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func position(
    by value: PlottableValue,
    axis: Axis? = nil,
    span: MarkDimension = .automatic
) -> some ChartContent where P : Plottable
```

## Parameters 

`value`  

The data used for positioning marks.

`axis`  

The axis to position marks along. Set this to `nil` to use a default configuration.

`span`  

The span of the positioned marks. Use this to control the total amount space available to the marks.

## Discussion

The code below creates a grouped bar chart that positions marks with the same “product” along the horizontal axis by their “type”.

```
Chart(cars) {
    BarMark(
        x: .value("product", $0.product),
        y: .value("price", $0.price)
    )
    .position(by: .value("type", $0.type), axis: .horizontal)
}
```

## See Also

### Encoding data into mark characteristics

func foregroundStyle&lt;D>(by: PlottableValue&lt;D>) -> some ChartContent

Represents data using a foreground style.

func lineStyle&lt;D>(by: PlottableValue&lt;D>) -> some ChartContent

Represents data using line styles.

func symbol&lt;D>(by: PlottableValue&lt;D>) -> some ChartContent

Represents data using different kinds of symbols.

func symbolSize&lt;D>(by: PlottableValue&lt;D>) -> some ChartContent

Represents data using symbol sizes.

