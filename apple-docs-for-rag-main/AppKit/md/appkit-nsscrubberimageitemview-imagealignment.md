

- AppKit
- NSScrubberImageItemView
-  imageAlignment 

Instance Property

# imageAlignment

The alignment of the image within the scrubber item.

macOS 10.12.2+

``` source
@MainActor
var imageAlignment: NSImageAlignment { get set }
```

## Discussion

The image is scaled proportionally to fit the frame of the item. This property determines how the image is cropped within that frame.

For possible values, see NSImageAlignment.

