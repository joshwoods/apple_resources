

- UIKit
-  NSDirectionalRectEdge 

Structure

# NSDirectionalRectEdge

Constants that specify an edge or a set of edges, taking the user interface layout direction into account.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct NSDirectionalRectEdge
```

## Topics

### Constants

static var top: NSDirectionalRectEdge

The top edge.

static var leading: NSDirectionalRectEdge

The leading edge.

static var bottom: NSDirectionalRectEdge

The bottom edge.

static var trailing: NSDirectionalRectEdge

The trailing edge.

static var all: NSDirectionalRectEdge

All edges.

### Initializers

init(rawValue: UInt)

Creates an edge with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

enum NSRectAlignment

Constants that specify alignment to an edge or a set of edges depending on the user interface layout direction.

struct UIDirectionalRectEdge

Constants that specify an edge or a set of edges, taking the user interface layout direction into account.

Deprecated

UIKit macros

Macros that UIKit defines.

