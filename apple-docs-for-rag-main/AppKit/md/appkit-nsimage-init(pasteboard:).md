

- AppKit
- NSImage
-  init(pasteboard:) 

Initializer

# init(pasteboard:)

Initializes and returns an image object with data from the specified pasteboard.

macOS

``` source
convenience init?(pasteboard: NSPasteboard)
```

## Parameters 

`pasteboard`  

The pasteboard containing the image data. The data on the pasteboard can be in any format that macOS supports, including PDF, PICT, EPS, or any number of bitmap data formats.

## Return Value

An initialized `NSImage` object or `nil` if the method cannot create an image from the contents of the pasteboard.

## Discussion

The specified pasteboard should contain a type supported by one of the registered `NSImageRep` subclasses. The table below lists the default pasteboard types and file extensions for several `NSImageRep` subclasses.

| Image representation class | Default pasteboard type | Default file extensions |
|----|----|----|
| `NSBitmapImageRep` | `NSTIFFPboardType` | `tiff`, `gif`, `jpg`, and others |
| `NSPDFImageRep` | `NSPDFPboardType` | `pdf` |
| `NSEPSImageRep` | `NSPostscriptPboardType` | `eps` |
| `NSPICTImageRep` | `NSPICTPboardType` | `pict` |

If the specified pasteboard contains the value `NSFilenamesPboardType`, each filename on the pasteboard should have an extension supported by one of the registered `NSImageRep` subclasses. You can use the imageUnfilteredFileTypes() method of a given subclass to obtain the list of supported types for that class.

## See Also

### Creating Images from Existing Data

convenience init?(data: Data)

Initializes and returns an image object using the provided image data.

convenience init?(dataIgnoringOrientation: Data)

Initializes and returns an image object using the provided image data and ignoring the EXIF orientation tags.

convenience init(cgImage: CGImage, size: NSSize)

Creates a new image using the contents of the provided image.

init(coder: NSCoder)

Initializes and returns an image object from data in an unarchiver.

