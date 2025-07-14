

- AppKit
- NSCursor
-  current 

Type Property

# current

Returns the application’s current cursor.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.0+

``` source
class var current: NSCursor { get }
```

## Return Value

The top cursor on the application’s cursor stack. This cursor may not be the visible cursor on the screen if a different application is currently active.

## Discussion

The method only returns the cursor set by your application using `NSCursor` methods. It does not return cursors set by other applications or cursors set by your application using Carbon APIs.

## See Also

### Related Documentation

func mouseEntered(with: NSEvent)

Automatically sent to the receiver when the cursor enters a cursor rectangle owned by the receiver.

Deprecated

func pop()

Sends a pop() message to the receiver’s class.

func push()

Puts the receiver on top of the cursor stack and makes it the current cursor.

func set()

Makes the receiver the current cursor.

func mouseExited(with: NSEvent)

Automatically sent to the receiver when the cursor exits a cursor rectangle owned by the receiver.

Deprecated

### Retrieving Cursor Instances

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

