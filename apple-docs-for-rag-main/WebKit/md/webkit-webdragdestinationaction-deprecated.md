

- WebKit
-  WebDragDestinationAction Deprecated

Structure

# WebDragDestinationAction

Actions that the destination object of a drag operation can perform.

macOS 10.3–10.14Deprecated

``` source
struct WebDragDestinationAction
```

## Topics

### Constants

static var DHTML: WebDragDestinationAction

Allows DHTML (such as JavaScript) to handle the drag.

static var edit: WebDragDestinationAction

Allows editable documents to be changed by the drag operation.

static var load: WebDragDestinationAction

Allows the drag operation to change the location.

static var any: WebDragDestinationAction

Allows any defined action to occur.

### Initializers

init(rawValue: UInt)

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

### Constants

Menu Item Tags

Tags that define the types of default menu items passed to the webView(_:contextMenuItemsForElement:defaultMenuItems:) method.

struct WebDragSourceAction

Actions that the source object of a drag operation can perform.

Deprecated

