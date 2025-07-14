

- AppKit
- NSImage
-  isValid 

Instance Property

# isValid

A Boolean value that indicates whether it is possible to draw an image representation.

macOS

``` source
var isValid: Bool { get }
```

## Discussion

If you created the image with an existing image file, but the corresponding image data is not yet loaded into memory, this method loads the data and expands it as needed. If the receiver contains no image representations and no associated image file, this method creates a valid cached image representation and initializes it to the default bit depth. If the file or URL from which the image was initialized is nonexistent, or the data in an existing file is invalid, this method returns false.

## See Also

### Related Documentation

convenience init?(byReferencingFile: String)

Initializes and returns an image object using the specified file.

convenience init(byReferencing: URL)

Initializes and returns an image object using the specified URL.

### Managing Drawing Options

var backgroundColor: NSColor

The background color for the image.

var capInsets: NSEdgeInsets

The cap insets for the image.

var resizingMode: NSImage.ResizingMode

The resizing mode for the image.

enum ResizingMode

Constants that describe the resizing mode for the image.

