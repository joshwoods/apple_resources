

- SwiftUI
- ZStack
-  init(alignment:spacing:content:) 

Initializer

# init(alignment:spacing:content:)

Creates an instance with the given spacing and alignment.

visionOS 2.0+

``` source
init(
    alignment: Alignment = .center,
    spacing: CGFloat?,
    @ViewBuilder content: () -> V
) where Content == ZStackContent3D, V : View
```

Available when `Content` conforms to `View`.

## Parameters 

`alignment`  

The guide for aligning the subviews in this stack on both the x- and y-axes.

`spacing`  

The distance between adjacent subviews, or `nil` if you want the stack to choose a default distance for each pair of subviews.

`content`  

A view builder that creates the content of this stack.

