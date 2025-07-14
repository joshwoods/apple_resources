

- AppKit
- NSImageRep
-  imagePasteboardTypes() Deprecated

Type Method

# imagePasteboardTypes()

Returns the pasteboard types supported by the image representation class or one of its subclasses.

macOS 10.0–10.10Deprecated

``` source
class func imagePasteboardTypes() -> [NSPasteboard.PasteboardType]
```

Deprecated

Use +imageTypes instead

## Return Value

An array of `NSString` objects, each of which contains a supported pasteboard format.

## Discussion

The list includes both those types returned by the imageUnfilteredPasteboardTypes() class method plus those that can be converted to a supported type by a user-installed filter service. Don’t override this method when subclassing `NSImageRep`—it always returns a valid list for any subclass of `NSImageRep` that correctly overrides the imageUnfilteredPasteboardTypes() method.

## See Also

### Determining Types for Images

class func canInit(with: Data) -> Bool

Returns a Boolean value that indicates whether the image representation can initialize itself from the specified data.

class func canInit(with: NSPasteboard) -> Bool

Returns a Boolean value that indicates whether the receiver can initialize itself from the data on the specified pasteboard.

class var imageTypes: [String]

Returns an array of UTI strings identifying the image types supported by the image representation, either directly or through a user-installed filter service.

class var imageUnfilteredTypes: [String]

Returns an array of UTI strings identifying the image types supported directly by the ime representation.

class func imageFileTypes() -> [String]

Returns the file types supported by the image representation class or one of its subclasses.

Deprecated

class func imageUnfilteredFileTypes() -> [String]

Returns the list of file types supported directly by the image representation.

Deprecated

class func imageUnfilteredPasteboardTypes() -> [NSPasteboard.PasteboardType]

Returns the list of pasteboard types supported directly by the image representation.

Deprecated

