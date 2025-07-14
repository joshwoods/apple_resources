

- SwiftUI
-  Edge3D 

Enumeration

# Edge3D

An edge or face of a 3D volume.

visionOS 1.0+

``` source
@frozen
enum Edge3D
```

## Topics

### Getting the edges

case top

case bottom

case leading

case trailing

case front

case back

### Creating an edge

init(Edge)

### Accessing sets of edges

struct Set

An efficient set of 3D edges.

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

enum Edge

An enumeration to indicate one edge of a rectangle.

enum HorizontalEdge

An edge on the horizontal axis.

enum VerticalEdge

An edge on the vertical axis.

struct EdgeInsets

The inset distances for the sides of a rectangle.

struct EdgeInsets3D

The inset distances for the faces of a 3D volume.

