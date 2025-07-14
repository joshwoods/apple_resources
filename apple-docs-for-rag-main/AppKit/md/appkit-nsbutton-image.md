

- AppKit
- NSButton
-  image 

Instance Property

# image

The image that appears on the button when it’s in an off state, or `nil` if there is no such image.

macOS

``` source
@MainActor
var image: NSImage? { get set }
```

## Discussion

The image contained in this property is always displayed on a button that doesn’t change its contents when highlighting or showing an on state. Buttons don’t display images by default.

## See Also

### Related Documentation

func setButtonType(NSButton.ButtonType)

Sets the button’s type, which affects its user interface and behavior when clicked.

### Configuring Button Images

var alternateImage: NSImage?

An alternate image that appears on the button when the button is in an on state.

var imagePosition: NSControl.ImagePosition

The position of the button’s image relative to its title.

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

