

- Swift Charts
- VectorizedChartContent
-  position(by:axis:span:) 

Instance Method

# position(by:axis:span:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func position(
    by value: PlottableProjection,
    axis: Axis? = nil,
    span: MarkDimension = .automatic
) -> some VectorizedChartContent
```

## See Also

### Styling marks

func foregroundStyle(KeyPath&lt;Self.DataElement, some ShapeStyle>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using a foreground style.

func opacity(KeyPath&lt;Self.DataElement, CGFloat>) -> some VectorizedChartContent&lt;Self.DataElement> 

func lineStyle(KeyPath&lt;Self.DataElement, StrokeStyle>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using line styles.

