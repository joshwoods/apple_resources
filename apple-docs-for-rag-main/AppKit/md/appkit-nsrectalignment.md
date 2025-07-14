

- AppKit
-  NSRectAlignment 

Enumeration

# NSRectAlignment

Constants that specify alignment to an edge or a set of edges depending on the user interface layout direction.

macOS 10.15+

``` source
enum NSRectAlignment
```

## Topics

### Alignments

case none

Has no specified alignment.

case top

Aligns to the top edge.

case topLeading

Aligns to the top and leading edges.

case leading

Aligns to the leading edge.

case bottomLeading

Aligns to the bottom and leading edges.

case bottom

Aligns to the bottom edge.

case bottomTrailing

Aligns to the bottom and trailing edges.

case trailing

Aligns to the trailing edge.

case topTrailing

Aligns to the top and trailing edges.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Related types

struct NSDirectionalEdgeInsets

The inset distances for views, taking the user interface layout direction into account.

struct NSDirectionalRectEdge

