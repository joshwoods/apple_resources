

- AppKit
- NSCursor
-  arrow 

Type Property

# arrow

Returns the default cursor, the arrow cursor.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.0+

``` source
class var arrow: NSCursor { get }
```

## Return Value

The default cursor, a slanted arrow with its hot spot at the tip. The arrow cursor is the one you’re used to seeing over buttons, scrollers, and many other objects in the window system.

## See Also

### Related Documentation

var hotSpot: NSPoint

The position of the click location within the cursor.

### Retrieving Cursor Instances

class var current: NSCursor

Returns the application’s current cursor.

class var currentSystem: NSCursor?

Returns the current system cursor.

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

