

- AppKit
- NSImage
-  init(cgImage:size:) 

Initializer

# init(cgImage:size:)

Creates a new image using the contents of the provided image.

macOS 10.6+

``` source
convenience init(
    cgImage: CGImage,
    size: NSSize
)
```

## Parameters 

`cgImage`  

The source image.

`size`  

The size of the new image. Use zero, or NSZeroSize in Objective-C, to have the new image adopt the pixel dimensions of the source image.

## Discussion

Don’t assume anything about the image, other than drawing it is equivalent to drawing the source image.

This is not a designated initializer.

## See Also

### Creating Images from Existing Data

convenience init?(data: Data)

Initializes and returns an image object using the provided image data.

convenience init?(dataIgnoringOrientation: Data)

Initializes and returns an image object using the provided image data and ignoring the EXIF orientation tags.

convenience init?(pasteboard: NSPasteboard)

Initializes and returns an image object with data from the specified pasteboard.

init(coder: NSCoder)

Initializes and returns an image object from data in an unarchiver.

