

- AppKit
- NSButtonCell
-  imagePosition 

Instance Property

# imagePosition

The position of the button’s image relative to its title.

macOS

``` source
@MainActor
var imagePosition: NSControl.ImagePosition { get set }
```

## Discussion

The value of this property is one of the image positions described in the “Constants” section of NSCell. If the title is above, below, or overlapping the image, or if there is no image, the text is horizontally centered within the button.

## See Also

### Related Documentation

var image: NSImage?

The image displayed by the cell, if any.

class NSButtonCell

An object that defines the user interface of a button or other clickable region of a view.

func setButtonType(NSButton.ButtonType)

Sets how the button highlights while pressed and how it shows its state.

### Managing Images

var alternateImage: NSImage?

The image the button displays in its alternate state.

var imageScaling: NSImageScaling

The scale factor for the button’s image.

