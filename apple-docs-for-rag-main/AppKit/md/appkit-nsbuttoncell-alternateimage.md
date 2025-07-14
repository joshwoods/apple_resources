

- AppKit
- NSButtonCell
-  alternateImage 

Instance Property

# alternateImage

The image the button displays in its alternate state.

macOS

``` source
@MainActor
var alternateImage: NSImage? { get set }
```

## Discussion

The value of this property is the image displayed by the button when it’s in its alternate state, or `nil` if there is no alternate image. Note that some button types don’t display an alternate image. Buttons don’t display images by default. Setting this property may redraw the contents of the button.

## See Also

### Related Documentation

var image: NSImage?

The image displayed by the cell, if any.

var keyEquivalent: String

The button’s key-equivalent character.

func setButtonType(NSButton.ButtonType)

Sets how the button highlights while pressed and how it shows its state.

### Managing Images

var imagePosition: NSControl.ImagePosition

The position of the button’s image relative to its title.

var imageScaling: NSImageScaling

The scale factor for the button’s image.

