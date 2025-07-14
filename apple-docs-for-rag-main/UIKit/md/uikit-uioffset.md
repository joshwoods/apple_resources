

- UIKit
-  UIOffset 

Structure

# UIOffset

A structure that specifies an amount to offset a position.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
struct UIOffset
```

## Overview

The components are positive for right or down, negative for left or up.

See also Initializing offsets and zero.

## Topics

### Initializing offsets

init(horizontal: CGFloat, vertical: CGFloat)

Creates an offset structure from the given components.

init()

Creates an offset structure.

### Getting the offset values

var horizontal: CGFloat

The amount of horizontal offset from a position.

var vertical: CGFloat

The amount of vertical offset from a position.

### Comparing offsets

func UIOffsetEqualToOffset(UIOffset, UIOffset) -> Bool

Returns a Boolean value that indicates whether two offsets are equal.

Deprecated

### Converting to and from strings

class func string(for: UIOffset) -> String

Returns a string formatted to contain the data from an offset structure.

class func uiOffset(for: String) -> UIOffset

Returns a UIKit offset structure corresponding to the data in a given string.

### Getting the empty offset value

static let zero: UIOffset

An offset structure with no offset in the horizontal and vertical directions.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Decodable
- Encodable
- Equatable
- Sendable

## See Also

### Related types

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

struct UIDirectionalRectEdge

Constants that specify an edge or a set of edges, taking the user interface layout direction into account.

Deprecated

UIKit macros

Macros that UIKit defines.

