

- AppKit
- NSImage
-  init(dataIgnoringOrientation:) 

Initializer

# init(dataIgnoringOrientation:)

Initializes and returns an image object using the provided image data and ignoring the EXIF orientation tags.

macOS 10.6+

``` source
convenience init?(dataIgnoringOrientation data: Data)
```

## Parameters 

`data`  

The data object containing the image data. The data can be in any format that macOS supports, including PDF, PICT, EPS, or any number of bitmap data formats.

## Return Value

An initialized `NSImage` object or `nil` if the method cannot create an image representation from the contents of the specified data object.

## See Also

### Creating Images from Existing Data

convenience init?(data: Data)

Initializes and returns an image object using the provided image data.

convenience init(cgImage: CGImage, size: NSSize)

Creates a new image using the contents of the provided image.

convenience init?(pasteboard: NSPasteboard)

Initializes and returns an image object with data from the specified pasteboard.

init(coder: NSCoder)

Initializes and returns an image object from data in an unarchiver.

