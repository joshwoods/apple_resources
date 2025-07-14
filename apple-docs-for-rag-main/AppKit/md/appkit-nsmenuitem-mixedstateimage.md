

- AppKit
- NSMenuItem
-  mixedStateImage 

Instance Property

# mixedStateImage

The image of the menu item that indicates a “mixed” state, that is, a state neither “on” nor “off.”

macOS

``` source
var mixedStateImage: NSImage! { get set }
```

## Discussion

A mixed state is useful for indicating a mix of “off” and “on” attribute values in a group of selected objects, such as a selection of text containing boldface and plain (non-boldface) words. By default this is a horizontal line.

## See Also

### Related Documentation

var state: NSControl.StateValue

The state of the menu item.

### Managing the image

var image: NSImage?

The menu item’s image.

var onStateImage: NSImage!

The image of the menu item that indicates an “on” state.

var offStateImage: NSImage?

The image of the menu item that indicates an “off” state.

