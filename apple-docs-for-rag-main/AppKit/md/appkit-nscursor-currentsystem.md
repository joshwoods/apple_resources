

- AppKit
- NSCursor
-  currentSystem 

Type Property

# currentSystem

Returns the current system cursor.

Mac Catalyst 13.1+macOS 10.6–15.4Deprecated

``` source
class var currentSystem: NSCursor? { get }
```

## Return Value

A cursor whose image and hot spot match those of the currently-displayed cursor on the system

## Discussion

This method returns the current system cursor regardless of which application set the cursor, and whether Cocoa or Carbon APIs were used to set it.

This method replaces the now deprecated QDGetCursorData function.

## See Also

### Retrieving Cursor Instances

class var current: NSCursor

Returns the application’s current cursor.

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

