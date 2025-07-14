

- UIKit
-  UIAxis 

Structure

# UIAxis

A structure that specifies the layout axes.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+tvOS 13.4+visionOS 1.0+watchOS 6.2+

``` source
struct UIAxis
```

## Topics

### Constants

static var horizontal: UIAxis

A value that represents the horizontal axis.

static var vertical: UIAxis

A value that represents the vertical axis.

static var both: UIAxis

A value that represents both axes.

### Initializers

init(rawValue: UInt)

Creates an axis with the specified raw value.

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

struct UIEdgeInsets

The inset distances for views.

struct NSDirectionalEdgeInsets

The inset distances for views, taking the user interface layout direction into account.

struct NSDirectionalRectEdge

Constants that specify an edge or a set of edges, taking the user interface layout direction into account.

enum NSRectAlignment

Constants that specify alignment to an edge or a set of edges depending on the user interface layout direction.

struct UIDirectionalRectEdge

Constants that specify an edge or a set of edges, taking the user interface layout direction into account.

Deprecated

UIKit macros

Macros that UIKit defines.

