

- AppKit
- NSImage
-  init(coder:) 

Initializer

# init(coder:)

Initializes and returns an image object from data in an unarchiver.

macOS

``` source
init(coder: NSCoder)
```

## See Also

### Creating Images from Existing Data

convenience init?(data: Data)

Initializes and returns an image object using the provided image data.

convenience init?(dataIgnoringOrientation: Data)

Initializes and returns an image object using the provided image data and ignoring the EXIF orientation tags.

convenience init(cgImage: CGImage, size: NSSize)

Creates a new image using the contents of the provided image.

convenience init?(pasteboard: NSPasteboard)

Initializes and returns an image object with data from the specified pasteboard.

