

- TVMLKit
- TVViewElement
-  updateType Deprecated

Instance Property

# updateType

The value that describes any changes to the DOM tree after it has been reparsed.

tvOS 9.0–18.0Deprecated

``` source
var updateType: TVElementUpdateType { get }
```

Deprecated

Please use SwiftUI or UIKit

## Discussion

For possible values, see TVElementUpdateType. This property is initially set to TVElementUpdateType.none.

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

enum TVElementUpdateType

Describes any changes to the DOM tree after it has been reparsed.

Deprecated

