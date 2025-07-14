

- UIKit
-  NSDirectionalEdgeInsets 

Structure

# NSDirectionalEdgeInsets

The inset distances for views, taking the user interface layout direction into account.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
struct NSDirectionalEdgeInsets
```

## Topics

### Creating directional edge insets

init(top: CGFloat, leading: CGFloat, bottom: CGFloat, trailing: CGFloat)

Creates a directional edge insets structure that contains the specified values.

init()

Creates a directional edge insets structure that contains default values.

init(EdgeInsets)

Creates a directional edge insets structure from a SwiftUI edge insets structure.

### Getting the edge values

var bottom: CGFloat

The bottom edge inset value.

var leading: CGFloat

The leading edge inset value.

var top: CGFloat

The top edge inset value.

var trailing: CGFloat

The trailing edge inset value.

### Converting to and from strings

class func string(for: NSDirectionalEdgeInsets) -> String

Returns a string formatted to contain the data from a directional edge insets structure.

class func nsDirectionalEdgeInsets(for: String) -> NSDirectionalEdgeInsets

Returns a directional edge insets structure based on data in the specified string.

### Getting the empty edge insets

static let zero: NSDirectionalEdgeInsets

A directional edge insets structure whose top, leading, bottom, and trailing fields all have a value of `0`.

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

struct UIEdgeInsets

The inset distances for views.

struct NSDirectionalRectEdge

Constants that specify an edge or a set of edges, taking the user interface layout direction into account.

enum NSRectAlignment

Constants that specify alignment to an edge or a set of edges depending on the user interface layout direction.

struct UIDirectionalRectEdge

Constants that specify an edge or a set of edges, taking the user interface layout direction into account.

Deprecated

UIKit macros

Macros that UIKit defines.

