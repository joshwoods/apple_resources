

- Swift Charts
- VectorizedChartContent
-  foregroundStyle(\_:) 

Instance Method

# foregroundStyle(\_:)

Represents data using a foreground style.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func foregroundStyle(_ keyPath: KeyPath) -> some VectorizedChartContent
```

## Parameters 

`keyPath`  

The accessor for shape style.

## See Also

### Styling marks

func opacity(KeyPath&lt;Self.DataElement, CGFloat>) -> some VectorizedChartContent&lt;Self.DataElement> 

func lineStyle(KeyPath&lt;Self.DataElement, StrokeStyle>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using line styles.

func position(by: PlottableProjection&lt;Self.DataElement, some Plottable>, axis: Axis?, span: MarkDimension) -> some VectorizedChartContent&lt;Self.DataElement> 

