

- AppKit
- NSMenuItem
-  image 

Instance Property

# image

The menu item’s image.

macOS

``` source
var image: NSImage? { get set }
```

## Discussion

The menu item’s image is not affected by changes in its state.

## See Also

### Managing the image

var onStateImage: NSImage!

The image of the menu item that indicates an “on” state.

var offStateImage: NSImage?

The image of the menu item that indicates an “off” state.

var mixedStateImage: NSImage!

The image of the menu item that indicates a “mixed” state, that is, a state neither “on” nor “off.”

