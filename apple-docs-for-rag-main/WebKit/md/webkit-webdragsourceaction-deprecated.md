

- WebKit
-  WebDragSourceAction Deprecated

Structure

# WebDragSourceAction

Actions that the source object of a drag operation can perform.

macOS 10.3–10.14Deprecated

``` source
struct WebDragSourceAction
```

## Topics

### Constants

static var DHTML: WebDragSourceAction

Allows DHTML (such as JavaScript) in the source object to initiate a drag operation.

static var image: WebDragSourceAction

Allows the user to drag an image in the source object.

static var link: WebDragSourceAction

Allows the user to drag a link in the source object.

static var selection: WebDragSourceAction

Allows the user to drag a selection in the source object.

static var any: WebDragSourceAction

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

struct WebDragDestinationAction

Actions that the destination object of a drag operation can perform.

Deprecated

