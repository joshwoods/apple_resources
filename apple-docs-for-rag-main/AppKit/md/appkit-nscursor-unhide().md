

- AppKit
- NSCursor
-  unhide() 

Type Method

# unhide()

Negates an earlier call to hide() by showing the current cursor.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.0+

``` source
class func unhide()
```

## Discussion

Each invocation of `unhide` must be balanced by an invocation of hide() in order for the cursor display to be correct.

## See Also

### Setting Cursor Attributes

var image: UIImage

The cursor’s image.

var hotSpot: NSPoint

The position of the click location within the cursor.

class func hide()

Makes the current cursor invisible.

class func setHiddenUntilMouseMoves(Bool)

Sets whether the cursor is hidden until the mouse moves.

