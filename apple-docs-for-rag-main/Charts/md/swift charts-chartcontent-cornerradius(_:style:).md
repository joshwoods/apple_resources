

- Swift Charts
- ChartContent
-  cornerRadius(\_:style:) 

Instance Method

# cornerRadius(\_:style:)

Sets the corner radius of the chart content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func cornerRadius(
    _ radius: CGFloat,
    style: RoundedCornerStyle = .continuous
) -> some ChartContent
```

## Parameters 

`radius`  

The corner radius.

`style`  

The style of the rounded corners.

## See Also

### Styling marks

func foregroundStyle&lt;S>(S) -> some ChartContent

Sets the foreground style for the chart content.

func opacity(Double) -> some ChartContent

Sets the opacity for the chart content.

func lineStyle(StrokeStyle) -> some ChartContent

Sets the style for line marks.

func interpolationMethod(InterpolationMethod) -> some ChartContent

Plots line and area marks with the interpolation method that you specify.

