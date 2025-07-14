

- AppKit
- NSCursor
-  image 

Instance Property

# image

The cursor’s image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.0+

**Mac Catalyst**

``` source
var image: UIImage { get }
```

**macOS**

``` source
var image: NSImage { get }
```

## Discussion

The cursor image or `nil` if none exists. Note that an `NSCursor` object is immutable: you cannot change its image after it’s created. Instead, use init(image:hotSpot:) to create a new cursor with the new settings.

## See Also

### Related Documentation

init(image: UIImage, hotSpot: NSPoint)

Initializes a cursor with the given image and hot spot.

### Setting Cursor Attributes

var hotSpot: NSPoint

The position of the click location within the cursor.

class func hide()

Makes the current cursor invisible.

class func unhide()

Negates an earlier call to hide() by showing the current cursor.

class func setHiddenUntilMouseMoves(Bool)

Sets whether the cursor is hidden until the mouse moves.

