

- AppKit
- NSControl
-  NSControl.ImagePosition 

Enumeration

# NSControl.ImagePosition

A constant for specifying the position of a button’s image relative to its title.

macOS

``` source
enum ImagePosition
```

## Overview

Use these constants with the imagePosition property of NSButton and NSButtonCell.

## Topics

### Positioning a Control’s Image

case noImage

The cell doesn’t display an image.

case imageOnly

The cell displays an image but not a title.

case imageLeading

The image is on the title’s leading edge.

case imageTrailing

The image is on the title’s trailing edge.

case imageLeft

The image is to the left of the title.

case imageRight

The image is to the right of the title.

case imageBelow

The image is below the title.

case imageAbove

The image is above the title.

case imageOverlaps

The image overlaps the title.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Button Images

var image: NSImage?

The image that appears on the button when it’s in an off state, or `nil` if there is no such image.

var alternateImage: NSImage?

An alternate image that appears on the button when the button is in an on state.

var imagePosition: NSControl.ImagePosition

The position of the button’s image relative to its title.

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

