

- AppKit
-  NSImageDelegate 

Protocol

# NSImageDelegate

A set of optional methods that you can use to respond to drawing failures and manage incremental loads.

macOS

``` source
protocol NSImageDelegate : NSObjectProtocol
```

## Topics

### Responding to Drawing Failure

func imageDidNotDraw(NSImage, in: NSRect) -> NSImage?

Tells the delegate that the image object is unable, for whatever reason, to lock focus on its image or draw in the specified rectangle.

### Managing Incremental Loads

enum LoadStatus

Status values for incremental image loading.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Images

Providing images for different appearances

Supply image resources appropriate for light and dark appearances and for high-contrast environments.

Supporting Continuity Camera in Your Mac App

Incorporate scanned documents and pictures from a user’s iPhone, iPad, or iPod touch into your Mac app using Continuity Camera.

Supporting HDR images in your app

​Load, display, edit, and save HDR images using SwiftUI and Core Image. ​

Applying Apple HDR effect to your photos

You can decode and apply Apple’s HDR gain map to your own images.

class NSImage

A high-level interface for manipulating image data.

class NSImageRep

A semiabstract superclass that provides subclasses that you use to draw an image from a particular type of source data.

