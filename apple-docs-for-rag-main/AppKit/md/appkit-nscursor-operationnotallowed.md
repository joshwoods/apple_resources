

- AppKit
- NSCursor
-  operationNotAllowed 

Type Property

# operationNotAllowed

Returns the operation not allowed cursor.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.5+

``` source
class var operationNotAllowed: NSCursor { get }
```

## Return Value

The operation not allowed cursor.

## Discussion

This cursor indicates that the operation that is being attempted, perhaps dragging to an item that can’t accept the drag type, is being denied.

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

class var disappearingItem: NSCursor

Returns a cursor indicating that the current operation will result in a disappearing item.

class var dragCopy: NSCursor

Returns a cursor indicating that the current operation will result in a copy action.

class var dragLink: NSCursor

Returns a cursor indicating that the current operation will result in a link action.

class var iBeam: NSCursor

Returns a cursor that looks like a capital I with a tiny crossbeam at its middle.

class var openHand: NSCursor

Returns the open-hand system cursor.

class var pointingHand: NSCursor

Returns the pointing-hand system cursor.

class var resizeDown: NSCursor

Returns the resize-down system cursor.

class var resizeLeft: NSCursor

Returns the resize-left system cursor.

class var resizeLeftRight: NSCursor

Returns the resize-left-and-right system cursor.

