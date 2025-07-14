

- Swift Charts
- ChartContent
-  mask(content:) 

Instance Method

# mask(content:)

Masks chart content using the alpha channel of the specified content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func mask(@ChartContentBuilder content: () -> C) -> some ChartContent where C : ChartContent
```

## Discussion

Parameter content: The content whose alpha will be applied to this item.

## See Also

### Masking and clipping

func clipShape(some Shape, style: FillStyle) -> some ChartContent

Sets a clip shape for the chart content.

