

- AppKit
- NSCursor
-  disappearingItem 

Type Property

# disappearingItem

Returns a cursor indicating that the current operation will result in a disappearing item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.0+

``` source
class var disappearingItem: NSCursor { get }
```

## Return Value

The system cursor that indicates that the current operation will result in a disappearing item (for example, when dragging an item from the dock or a toolbar).

## See Also

### Retrieving Cursor Instances

class var current: NSCursor

Returns the application’s current cursor.

class var currentSystem: NSCursor?

Returns the current system cursor.

class var arrow: NSCursor

Returns the default cursor, the arrow cursor.

class var contextualMenu: NSCursor

Returns the contextual menu system cursor.

class var closedHand: NSCursor

Returns the closed-hand system cursor.

class var crosshair: NSCursor

Returns the cross-hair system cursor.

class var dragCopy: NSCursor

Returns a cursor indicating that the current operation will result in a copy action.

class var dragLink: NSCursor

Returns a cursor indicating that the current operation will result in a link action.

class var iBeam: NSCursor

Returns a cursor that looks like a capital I with a tiny crossbeam at its middle.

class var openHand: NSCursor

Returns the open-hand system cursor.

class var operationNotAllowed: NSCursor

Returns the operation not allowed cursor.

class var pointingHand: NSCursor

Returns the pointing-hand system cursor.

class var resizeDown: NSCursor

Returns the resize-down system cursor.

class var resizeLeft: NSCursor

Returns the resize-left system cursor.

class var resizeLeftRight: NSCursor

Returns the resize-left-and-right system cursor.

