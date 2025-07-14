

- AppKit
- NSButton
-  showsBorderOnlyWhileMouseInside 

Instance Property

# showsBorderOnlyWhileMouseInside

A Boolean value that determines whether the button displays its border only when the pointer is over it.

macOS

``` source
@MainActor
var showsBorderOnlyWhileMouseInside: Bool { get set }
```

## Discussion

The value of this property is true if the button’s border is displayed only when the pointer is over the button and the button is active. The value is false if the border is displayed all the time, regardless of the position of the pointer. By default, this method returns false.

If isBordered is false, the border is never displayed, regardless of the value of showsBorderOnlyWhileMouseInside.

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

var imageHugsTitle: Bool

A Boolean value that determines how the button’s image and title are positioned together within the button bezel.

var imageScaling: NSImageScaling

The scaling mode applied to make the cell’s image fit the frame of the image view.

