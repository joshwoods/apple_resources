

- AppKit
- NSCursor
-  hotSpot 

Instance Property

# hotSpot

The position of the click location within the cursor.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.0+

``` source
var hotSpot: NSPoint { get }
```

## Discussion

The hot spot precisely determines the click location within the cursor’s image. Using its flipped coordinate system, you calculate the hot spot in points with the top-left corner acting as the origin. For example, the arrow cursor’s hot spot is at the intersection of its left and right edges, which is inset 4pts from the image’s corner to account for the arrow’s stroke and shadow.

Note that an `NSCursor` object is immutable: you can’t change its hot spot after it’s created. Instead, use init(image:hotSpot:) to create a new cursor with the new settings.

## See Also

### Related Documentation

init(image: UIImage, hotSpot: NSPoint)

Initializes a cursor with the given image and hot spot.

### Setting Cursor Attributes

var image: UIImage

The cursor’s image.

class func hide()

Makes the current cursor invisible.

class func unhide()

Negates an earlier call to hide() by showing the current cursor.

class func setHiddenUntilMouseMoves(Bool)

Sets whether the cursor is hidden until the mouse moves.

