

- SwiftUI
-  Edge 

Enumeration

# Edge

An enumeration to indicate one edge of a rectangle.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
enum Edge
```

## Topics

### Getting the edges

case top

case bottom

case leading

case trailing

### Creating an edge

init?(Edge3D)

Converts a 3D edge to a 2D edge, if possible.

### Accessing sets of edges

struct Set

An efficient set of edges.

## Relationships

### Conforms To

- BitwiseCopyable
- CaseIterable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing edges and regions

enum Edge3D

An edge or face of a 3D volume.

enum HorizontalEdge

An edge on the horizontal axis.

enum VerticalEdge

An edge on the vertical axis.

struct EdgeInsets

The inset distances for the sides of a rectangle.

struct EdgeInsets3D

The inset distances for the faces of a 3D volume.

