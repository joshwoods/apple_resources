

- Swift Charts
- AxisContent
-  compositingLayer(style:) 

Instance Method

# compositingLayer(style:)

Creates a compositing layer for the chart content, and apply view modifiers to the compositing layer.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func compositingLayer(@ViewBuilder style: (PlaceholderContentView) -> V) -> some AxisContent where V : View
```

## Parameters 

`style`  

A closure that applies view modifiers to the compositing layer.

