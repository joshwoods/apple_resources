

- AppKit
- NSCursor
-  init(image:foregroundColorHint:backgroundColorHint:hotSpot:) Deprecated

Initializer

# init(image:foregroundColorHint:backgroundColorHint:hotSpot:)

Initializes the cursor with the specified image and hot spot.

macOS 10.0–10.12Deprecated

``` source
convenience init(
    image newImage: NSImage,
    foregroundColorHint fg: NSColor?,
    backgroundColorHint bg: NSColor?,
    hotSpot: NSPoint
)
```

Deprecated

Color hints are ignored. Use init(image:hotSpot:) instead.

## Parameters 

`newImage`  

The image to assign to the cursor.

`fg`  

The foreground color. This is currently ignored.

`bg`  

The background color. This is currently ignored.

`hotSpot`  

The point to assign as the cursor’s hot spot.

## Return Value

The initialized cursor object.

## See Also

### Initializing a New Cursor

init(image: UIImage, hotSpot: NSPoint)

Initializes a cursor with the given image and hot spot.

