

- Swift Charts
- VectorizedChartContent
-  opacity(\_:) 

Instance Method

# opacity(\_:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func opacity(_ keyPath: KeyPath) -> some VectorizedChartContent
```

## Parameters 

`keyPath`  

Points to a value between 0 (fully transparent) and 1 (fully opaque).

## See Also

### Styling marks

func foregroundStyle(KeyPath&lt;Self.DataElement, some ShapeStyle>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using a foreground style.

func lineStyle(KeyPath&lt;Self.DataElement, StrokeStyle>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using line styles.

func position(by: PlottableProjection&lt;Self.DataElement, some Plottable>, axis: Axis?, span: MarkDimension) -> some VectorizedChartContent&lt;Self.DataElement> 

