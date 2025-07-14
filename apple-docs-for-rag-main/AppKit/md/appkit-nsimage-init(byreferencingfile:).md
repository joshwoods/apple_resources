

- AppKit
- NSImage
-  init(byReferencingFile:) 

Initializer

# init(byReferencingFile:)

Initializes and returns an image object using the specified file.

macOS

``` source
convenience init?(byReferencingFile fileName: String)
```

## Parameters 

`fileName`  

A full or relative path name specifying the file with the desired image data. Relative paths must be relative to the current working directory.

## Return Value

An initialized `NSImage` object or `nil` if the new object cannot be initialized.

## Discussion

This method initializes the image object lazily. It does not actually open the specified file or create any image representations from its data until an app attempts to draw the image or request information about it.

The `filename` parameter should include the file extension that identifies the type of the image data. The mechanism that actually creates the image representation for `filename` looks for an `NSImageRep` subclass that handles that data type from among those registered with `NSImage`.

Because this method doesn’t actually create image representations for the image data, your app should do error checking before attempting to use the image; one way to do so is by accessing the isValid property to check whether the image can be drawn.

This method invokes setDataRetained: with an argument of true, thus enabling it to hold onto its filename. When archiving an image created with this method, only the image’s filename is written to the archive.

If the cached version of the image uses less memory than the original image data, AppKit deletes the original data and uses the cached image. (This can occur for images whose resolution is greater than 72 dpi.) If you resize the image by less than 50%, AppKit loads the data in again from the file. If you expect to delete the file or change its contents, use init(contentsOfFile:) instead.

## See Also

### Related Documentation

Cocoa Drawing Guide

### Creating Images from Resource Files

convenience init(byReferencing: URL)

Initializes and returns an image object using the specified URL.

convenience init?(contentsOfFile: String)

Initializes and returns an image object with the contents of the specified file.

convenience init?(contentsOf: URL)

Initializes and returns an image object with the contents of the specified URL.

