

- AppKit
- NSButton
-  imageHugsTitle 

Instance Property

# imageHugsTitle

A Boolean value that determines how the button’s image and title are positioned together within the button bezel.

macOS 10.12+

``` source
@MainActor
var imageHugsTitle: Bool { get set }
```

## Discussion

When the value of this property is false (the default value), the button’s image is positioned according to the imagePosition property at the edge of the button bezel, and the title is positioned within the remaining space.

When this property is true, the button’s image is positioned directly adjacent to the title based on the imagePosition property, and the image and title are positioned within the button bezel as a single unit.

## See Also

### Configuring Button Images

var image: NSImage?

The image that appears on the button when it’s in an off state, or `nil` if there is no such image.

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

var imageScaling: NSImageScaling

The scaling mode applied to make the cell’s image fit the frame of the image view.

