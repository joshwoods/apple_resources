

- SwiftUI
- LayoutSubview
-  sizeThatFits(\_:) 

Instance Method

# sizeThatFits(\_:)

Asks the subview for its size.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func sizeThatFits(_ proposal: ProposedViewSize) -> CGSize
```

## Parameters 

`proposal`  

A proposed size for the subview. In SwiftUI, views choose their own size, but can take a size proposal from their parent view into account when doing so.

## Return Value

The size that the subview chooses for itself, given the proposal from its container view.

## Discussion

Use this method as a convenience to get the width and height properties of the ViewDimensions instance returned by the dimensions(in:) method, reported as a CGSize instance.

## See Also

### Getting subview characteristics

func dimensions(in: ProposedViewSize) -> ViewDimensions

Asks the subview for its dimensions and alignment guides.

var spacing: ViewSpacing

The subviews’s preferred spacing values.

var priority: Double

The layout priority of the subview.

