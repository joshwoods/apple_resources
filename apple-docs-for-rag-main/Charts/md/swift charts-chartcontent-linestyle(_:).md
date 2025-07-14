

- Swift Charts
- ChartContent
-  lineStyle(\_:) 

Instance Method

# lineStyle(\_:)

Sets the style for line marks.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func lineStyle(_ style: StrokeStyle) -> some ChartContent
```

## Parameters 

`style`  

The stroke style.

## Discussion

Warning

Use this `.lineStyle(_:)` overload only if you have a predefined stroke style. The provided stroke style will override default line width and line cap for line marks.

## See Also

### Styling marks

func foregroundStyle&lt;S>(S) -> some ChartContent

Sets the foreground style for the chart content.

func opacity(Double) -> some ChartContent

Sets the opacity for the chart content.

func cornerRadius(CGFloat, style: RoundedCornerStyle) -> some ChartContent

Sets the corner radius of the chart content.

func interpolationMethod(InterpolationMethod) -> some ChartContent

Plots line and area marks with the interpolation method that you specify.

