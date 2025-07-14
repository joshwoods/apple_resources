

- UIKit
-  UIEdgeInsets 

Structure

# UIEdgeInsets

The inset distances for views.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS 2.0+

``` source
struct UIEdgeInsets
```

## Overview

Edge inset values are applied to a rectangle to shrink or expand the area represented by that rectangle. Typically, edge insets are used during view layout to modify the view’s frame. Positive values cause the frame to be inset (or shrunk) by the specified amount. Negative values cause the frame to be outset (or expanded) by the specified amount.

See also init(top:left:bottom:right:) and zero.

## Topics

### Creating edge insets

init(top: CGFloat, left: CGFloat, bottom: CGFloat, right: CGFloat)

Creates an edge insets structure with the specified edges.

init()

Initializes the edge insets structure to default values.

### Getting the edge values

var bottom: CGFloat

The bottom edge inset value.

var left: CGFloat

The left edge inset value.

var right: CGFloat

The right edge inset value.

var top: CGFloat

The top edge inset value.

### Managing edge insets

func inset(by insets: UIEdgeInsets) -> CGRect

### Converting to and from strings

class func string(for: UIEdgeInsets) -> String

Returns a string formatted to contain the data from an edge insets structure.

class func uiEdgeInsets(for: String) -> UIEdgeInsets

Returns a UIKit edge insets structure based on the data in the specified string.

### Getting the empty edge insets

static let zero: UIEdgeInsets

An edge insets struct whose top, left, bottom, and right fields are all set to `0`.

### Comparing edge insets

func UIEdgeInsetsEqualToEdgeInsets(UIEdgeInsets, UIEdgeInsets) -> Bool

Returns a Boolean value indicating whether the two edge insets are the same.

Deprecated

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

struct UIOffset

A structure that specifies an amount to offset a position.

struct UIAxis

A structure that specifies the layout axes.

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

