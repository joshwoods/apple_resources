

- Swift Charts
- ChartContent
-  foregroundStyle(\_:) 

Instance Method

# foregroundStyle(\_:)

Sets the foreground style for the chart content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func foregroundStyle(_ style: S) -> some ChartContent where S : ShapeStyle
```

## Parameters 

`style`  

The shape style.

## See Also

### Styling marks

func opacity(Double) -> some ChartContent

Sets the opacity for the chart content.

func cornerRadius(CGFloat, style: RoundedCornerStyle) -> some ChartContent

Sets the corner radius of the chart content.

func lineStyle(StrokeStyle) -> some ChartContent

Sets the style for line marks.

func interpolationMethod(InterpolationMethod) -> some ChartContent

Plots line and area marks with the interpolation method that you specify.

