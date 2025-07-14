

- SwiftUI
- Shape
-  sizeThatFits(\_:) 

Instance Method

# sizeThatFits(\_:)

Returns the size of the view that will render the shape, given a proposed size.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func sizeThatFits(_ proposal: ProposedViewSize) -> CGSize
```

**Required** Default implementation provided.

## Parameters 

`proposal`  

A size proposal for the container.

## Return Value

A size that indicates how much space the shape needs.

## Discussion

Implement this method to tell the container of the shape how much space the shape needs to render itself, given a size proposal.

See sizeThatFits(proposal:subviews:cache:) for more details about how the layout system chooses the size of views.

## Default Implementations

### Shape Implementations

func sizeThatFits(ProposedViewSize) -> CGSize

Returns the original proposal, with nil components replaced by a small positive value.

## See Also

### Defining a shape’s size and path

func path(in: CGRect) -> Path

Describes this shape as a path within a rectangular frame of reference.

**Required**

