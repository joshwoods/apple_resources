

- AppKit
- NSCursor
-  init(image:hotSpot:) 

Initializer

# init(image:hotSpot:)

Initializes a cursor with the given image and hot spot.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.0+

**Mac Catalyst**

``` source
init(
    image newImage: UIImage,
    hotSpot point: NSPoint
)
```

**macOS**

``` source
init(
    image newImage: NSImage,
    hotSpot point: NSPoint
)
```

## Parameters 

`newImage`  

The image to assign to the cursor.

`point`  

The point to set as the cursor’s hot spot.

## Return Value

An initialized cursor object.

## Discussion

This method is the designated initializer for the class.

## See Also

### Related Documentation

var image: UIImage

The cursor’s image.

Cursor Management

var hotSpot: NSPoint

The position of the click location within the cursor.

### Initializing a New Cursor

convenience init(image: NSImage, foregroundColorHint: NSColor?, backgroundColorHint: NSColor?, hotSpot: NSPoint)

Initializes the cursor with the specified image and hot spot.

Deprecated

