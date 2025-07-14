

- AppKit
- NSButton
-  isBordered 

Instance Property

# isBordered

A Boolean value that determines whether the button has a border.

macOS

``` source
@MainActor
var isBordered: Bool { get set }
```

## Discussion

The value of this property is true if the button has a border, false otherwise. A button’s border isn’t the single line of most other controls’ borders—instead, it’s a raised bezel. By default, buttons are bordered. If the bordered state of a button changes, it gets redrawn.

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

