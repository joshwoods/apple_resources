

- AppKit
- NSImage
-  imageTypes 

Type Property

# imageTypes

Returns an array of UTI strings identifying the image types supported by the registered image representation objects, either directly or through a user-installed filter service.

macOS 10.5+

``` source
class var imageTypes: [String] { get }
```

## Return Value

An array of `NSString` objects, each of which contains a UTI identifying a supported image type. Some sample image-related UTI strings include “`public.image`”, “`public.jpeg`”, and “`public.tiff`”. For a list of supported types, see `UTCoreTypes.h`.

## Discussion

The returned list includes UTIs all file types supported by registered subclasses of `NSImageRep` plus those that can be converted to a supported type by a user-installed filter service. You can use the returned UTI strings with any method that supports UTIs.

Do not override this method directly. If your app supports custom image types, create and register an NSImageRep subclass that handles those types.

## See Also

### Determining Supported Types of Images

class func canInit(with: NSPasteboard) -> Bool

Tests whether the image can create an instance of itself using pasteboard data.

class var imageUnfilteredTypes: [String]

Returns an array of UTI strings identifying the image types supported directly by the registered image representation objects.

