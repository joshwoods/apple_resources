

- SwiftUI
- Shape
-  path(in:) 

Instance Method

# path(in:)

Describes this shape as a path within a rectangular frame of reference.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func path(in rect: CGRect) -> Path
```

**Required**

## Parameters 

`rect`  

The frame of reference for describing this shape.

## Return Value

A path that describes this shape.

## See Also

### Defining a shape’s size and path

func sizeThatFits(ProposedViewSize) -> CGSize

Returns the size of the view that will render the shape, given a proposed size.

**Required** Default implementation provided.

