

- AppKit
- NSCursor
-  hide() 

Type Method

# hide()

Makes the current cursor invisible.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.0+

``` source
class func hide()
```

## Discussion

If another cursor becomes current, that cursor will be invisible, too. It will remain invisible until you invoke the unhide() method.

Each invocation of `hide` must be balanced by an invocation of unhide() in order for the cursor to be displayed.

The hide() method overrides setHiddenUntilMouseMoves(_:).

## See Also

### Setting Cursor Attributes

var image: UIImage

The cursor’s image.

var hotSpot: NSPoint

The position of the click location within the cursor.

class func unhide()

Negates an earlier call to hide() by showing the current cursor.

class func setHiddenUntilMouseMoves(Bool)

Sets whether the cursor is hidden until the mouse moves.

