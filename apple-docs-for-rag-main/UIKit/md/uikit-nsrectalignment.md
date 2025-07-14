

- UIKit
-  NSRectAlignment 

Enumeration

# NSRectAlignment

Constants that specify alignment to an edge or a set of edges depending on the user interface layout direction.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

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

struct UIOffset

A structure that specifies an amount to offset a position.

struct UIAxis

A structure that specifies the layout axes.

struct UIEdgeInsets

The inset distances for views.

struct NSDirectionalEdgeInsets

The inset distances for views, taking the user interface layout direction into account.

struct NSDirectionalRectEdge

Constants that specify an edge or a set of edges, taking the user interface layout direction into account.

struct UIDirectionalRectEdge

Constants that specify an edge or a set of edges, taking the user interface layout direction into account.

Deprecated

UIKit macros

Macros that UIKit defines.

