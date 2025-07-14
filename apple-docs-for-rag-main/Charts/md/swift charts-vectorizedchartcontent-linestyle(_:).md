

- Swift Charts
- VectorizedChartContent
-  lineStyle(\_:) 

Instance Method

# lineStyle(\_:)

Represents data using line styles.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func lineStyle(_ style: KeyPath) -> some VectorizedChartContent
```

## Parameters 

`style`  

The keyPath accessor for shape style.

## See Also

### Styling marks

func foregroundStyle(KeyPath&lt;Self.DataElement, some ShapeStyle>) -> some VectorizedChartContent&lt;Self.DataElement> 

Represents data using a foreground style.

func opacity(KeyPath&lt;Self.DataElement, CGFloat>) -> some VectorizedChartContent&lt;Self.DataElement> 

func position(by: PlottableProjection&lt;Self.DataElement, some Plottable>, axis: Axis?, span: MarkDimension) -> some VectorizedChartContent&lt;Self.DataElement> 

