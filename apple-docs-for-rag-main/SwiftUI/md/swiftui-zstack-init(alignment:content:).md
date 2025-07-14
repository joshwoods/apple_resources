

- SwiftUI
- ZStack
-  init(alignment:content:) 

Initializer

# init(alignment:content:)

Creates an instance with the given alignment.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    alignment: Alignment = .center,
    @ViewBuilder content: () -> Content
)
```

## Parameters 

`alignment`  

The guide for aligning the subviews in this stack on both the x- and y-axes.

`content`  

A view builder that creates the content of this stack.

