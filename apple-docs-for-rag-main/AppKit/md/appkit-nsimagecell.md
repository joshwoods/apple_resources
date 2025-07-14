

- AppKit
-  NSImageCell 

Class

# NSImageCell

An `NSImageCell` object displays a single image (encapsulated in an NSImage object) in a frame. This class provides methods for choosing the frame and for aligning and scaling the image to fit the frame.

macOS

``` source
@MainActor
class NSImageCell
```

## Overview

The object value of an `NSImageCell` object must be an NSImage object, so if you use the objectValue method of NSCell, be sure to supply an NSImage object as an argument. Because an NSImage object does not need to be converted for display, do not use the NSCell methods relating to formatters.

An `NSImageCell` object is usually associated with some kind of control object. For example, an NSMatrix or an NSTableView.

### Designated Initializers

When subclassing `NSImageCell` you must implement all of the designated initializers. Those methods are: init, init(coder:), init(textCell:), and init(imageCell:).

## Topics

### Aligning and Scaling the Image

var imageAlignment: NSImageAlignment

The alignment of the receiver’s image relative to its frame.

var imageScaling: NSImageScaling

The scaling mode used to fit the receiver’s image into the frame.

### Choosing the Frame

var imageFrameStyle: NSImageView.FrameStyle

The style of the frame that borders the image.

### Constants

enum NSImageAlignment

Constants used by imageAlignment that allow you to specify the location of the image in the frame.

enum FrameStyle

Constants that allow you to specify the kind of frame bordering the image.

## Relationships

### Inherits From

- NSCell

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSCoding
- NSCopying
- NSObjectProtocol
- NSUserInterfaceItemIdentification
- Sendable

