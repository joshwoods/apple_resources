

- AppKit
- NSButton
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

If the title is above, below, or overlapping the image, or if there is no image, the text is horizontally centered within the button. See NSControl.ImagePosition in NSCell for the list of possible image positions.

## See Also

### Related Documentation

var title: String

The title displayed on the button when it’s in an off state.

func setButtonType(NSButton.ButtonType)

Sets the button’s type, which affects its user interface and behavior when clicked.

### Configuring Button Images

var image: NSImage?

The image that appears on the button when it’s in an off state, or `nil` if there is no such image.

var alternateImage: NSImage?

An alternate image that appears on the button when the button is in an on state.

enum ImagePosition

A constant for specifying the position of a button’s image relative to its title.

var isBordered: Bool

A Boolean value that determines whether the button has a border.

var isTransparent: Bool

A Boolean value that indicates whether the button is transparent.

var bezelStyle: NSButton.BezelStyle

The appearance of the button’s border.

var bezelColor: NSColor?

The color of the button’s bezel, in appearances that support it.

var showsBorderOnlyWhileMouseInside: Bool

A Boolean value that determines whether the button displays its border only when the pointer is over it.

var imageHugsTitle: Bool

A Boolean value that determines how the button’s image and title are positioned together within the button bezel.

var imageScaling: NSImageScaling

The scaling mode applied to make the cell’s image fit the frame of the image view.

