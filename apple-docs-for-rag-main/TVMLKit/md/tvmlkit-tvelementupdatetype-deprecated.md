

- TVMLKit
-  TVElementUpdateType Deprecated

Enumeration

# TVElementUpdateType

Describes any changes to the DOM tree after it has been reparsed.

tvOS 9.0–18.0Deprecated

``` source
enum TVElementUpdateType
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Constants

case none

The tree structure did not change.

case subtree

A subtree element has been updated without affecting the order of any immediate children.

case children

The order of child nodes have been updated due to the addition, removal, or replacement of child nodes.

case node

The current node and its subtree have been modified.

### Enumeration Cases

case styles

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

### Inspecting a View Element

var autoHighlightIdentifier: String?

A string identifying the element that is initially in focus.

Deprecated

var attributes: [String : String]?

The attributes associated with a view element.

Deprecated

var children: [TVViewElement]?

An array containing the child elements of the element currently being inspected.

Deprecated

var isDisabled: Bool

Boolean value indicating whether the current element being inspected is disabled.

Deprecated

var identifier: String

A string containing the unique identifier for an element.

Deprecated

var name: String

A string containing the element’s name.

Deprecated

var parent: TVViewElement?

The parent of the current node.

Deprecated

var style: TVViewElementStyle?

The style applied to an element.

Deprecated

var updateType: TVElementUpdateType

The value that describes any changes to the DOM tree after it has been reparsed.

Deprecated

