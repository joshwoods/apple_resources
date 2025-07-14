

- AppKit
- NSImageRep
-  imageTypes 

Type Property

# imageTypes

Returns an array of UTI strings identifying the image types supported by the image representation, either directly or through a user-installed filter service.

macOS 10.5+

``` source
class var imageTypes: [String] { get }
```

## Return Value

An array of `NSString` objects, each of which contains a UTI identifying a supported image type. Some sample image-related UTI strings include “`public.image`”, “`public.jpeg`”, and “`public.tiff`”. For a list of supported types, see `UTCoreTypes.h`.

## Discussion

The returned list includes UTIs all file types supported by this image representation object plus those that can be opened by this image representation after being converted by a user-installed filter service. You can use the returned UTI strings with any method that supports UTIs.

## See Also

### Determining Types for Images

class func canInit(with: Data) -> Bool

Returns a Boolean value that indicates whether the image representation can initialize itself from the specified data.

class func canInit(with: NSPasteboard) -> Bool

Returns a Boolean value that indicates whether the receiver can initialize itself from the data on the specified pasteboard.

class var imageUnfilteredTypes: [String]

Returns an array of UTI strings identifying the image types supported directly by the ime representation.

class func imageFileTypes() -> [String]

Returns the file types supported by the image representation class or one of its subclasses.

Deprecated

class func imagePasteboardTypes() -> [NSPasteboard.PasteboardType]

Returns the pasteboard types supported by the image representation class or one of its subclasses.

Deprecated

class func imageUnfilteredFileTypes() -> [String]

Returns the list of file types supported directly by the image representation.

Deprecated

class func imageUnfilteredPasteboardTypes() -> [NSPasteboard.PasteboardType]

Returns the list of pasteboard types supported directly by the image representation.

Deprecated

