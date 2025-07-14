

- UIKit
-  UIDirectionalRectEdge Deprecated

Structure

# UIDirectionalRectEdge

Constants that specify an edge or a set of edges, taking the user interface layout direction into account.

iOS 13.0–13.0DeprecatediPadOS 13.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 13.0–13.0DeprecatedwatchOS 6.0–6.0Deprecated

``` source
struct UIDirectionalRectEdge
```

Deprecated

Use NSDirectionalRectEdge instead.

## Topics

### Constants

static var top: UIDirectionalRectEdge

The top edge.

static var leading: UIDirectionalRectEdge

The leading edge.

static var bottom: UIDirectionalRectEdge

The bottom edge.

static var trailing: UIDirectionalRectEdge

The trailing edge.

static var all: UIDirectionalRectEdge

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

struct NSDirectionalRectEdge

Constants that specify an edge or a set of edges, taking the user interface layout direction into account.

enum NSRectAlignment

Constants that specify alignment to an edge or a set of edges depending on the user interface layout direction.

UIKit macros

Macros that UIKit defines.

