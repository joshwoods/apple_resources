

- SwiftUI
- LazyHStack
-  init(alignment:spacing:pinnedViews:content:) 

Initializer

# init(alignment:spacing:pinnedViews:content:)

Creates a lazy horizontal stack view with the given spacing, vertical alignment, pinning behavior, and content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(
    alignment: VerticalAlignment = .center,
    spacing: CGFloat? = nil,
    pinnedViews: PinnedScrollableViews = .init(),
    @ViewBuilder content: () -> Content
)
```

## Parameters 

`alignment`  

The guide for aligning the subviews in this stack. All child views have the same vertical screen coordinate.

`spacing`  

The distance between adjacent subviews, or `nil` if you want the stack to choose a default distance for each pair of subviews.

`pinnedViews`  

The kinds of child views that will be pinned.

`content`  

A view builder that creates the content of this stack.

