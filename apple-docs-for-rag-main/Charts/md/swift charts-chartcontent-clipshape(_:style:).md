

- Swift Charts
- ChartContent
-  clipShape(\_:style:) 

Instance Method

# clipShape(\_:style:)

Sets a clip shape for the chart content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func clipShape(
    _ shape: some Shape,
    style: FillStyle = FillStyle()
) -> some ChartContent
```

## Parameters 

`shape`  

The clip shape. The shape fills each mark’s frame.

`style`  

The fill to use when rasterizing the shape.

## See Also

### Masking and clipping

func mask&lt;C>(content: () -> C) -> some ChartContent

Masks chart content using the alpha channel of the specified content.

