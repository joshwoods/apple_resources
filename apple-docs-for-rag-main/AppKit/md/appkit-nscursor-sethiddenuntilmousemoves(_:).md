

- AppKit
- NSCursor
-  setHiddenUntilMouseMoves(\_:) 

Type Method

# setHiddenUntilMouseMoves(\_:)

Sets whether the cursor is hidden until the mouse moves.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.0+

``` source
class func setHiddenUntilMouseMoves(_ flag: Bool)
```

## Parameters 

`flag`  

true to hide the cursor until one of the following occurs:

- The mouse moves.

- You invoke the method again, with `flag` set to false.

## Discussion

Do not try to counter this method by invoking unhide(). The results are undefined.

## See Also

### Setting Cursor Attributes

var image: UIImage

The cursor’s image.

var hotSpot: NSPoint

The position of the click location within the cursor.

class func hide()

Makes the current cursor invisible.

class func unhide()

Negates an earlier call to hide() by showing the current cursor.

