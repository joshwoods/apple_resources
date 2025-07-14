

- AppKit
-  NSDirectionalEdgeInsets 

Structure

# NSDirectionalEdgeInsets

The inset distances for views, taking the user interface layout direction into account.

macOS 10.15+

``` source
struct NSDirectionalEdgeInsets
```

## Topics

### Creating directional edge insets

init()

Creates a directional edge insets structure that contains default values.

init(top: CGFloat, leading: CGFloat, bottom: CGFloat, trailing: CGFloat)

Creates a directional edge insets structure that contains the specified values.

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

let NSDirectionalEdgeInsetsZero: NSDirectionalEdgeInsets

A directional edge insets structure whose top, leading, bottom, and trailing fields all have a value of `0`.

### Initializers

init(EdgeInsets)

Create edge insets from the equivalent EdgeInsets.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Related types

enum NSRectAlignment

Constants that specify alignment to an edge or a set of edges depending on the user interface layout direction.

struct NSDirectionalRectEdge

