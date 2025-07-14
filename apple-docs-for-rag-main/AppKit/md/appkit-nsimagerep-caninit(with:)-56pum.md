

- AppKit
- NSImageRep
-  canInit(with:) 

Type Method

# canInit(with:)

Returns a Boolean value that indicates whether the receiver can initialize itself from the data on the specified pasteboard.

macOS

``` source
class func canInit(with pasteboard: NSPasteboard) -> Bool
```

## Parameters 

`pasteboard`  

The pasteboard containing the image data.

## Return Value

true if the receiver understands the format of the specified data and can use it to initialize itself; otherwise, false.

## Discussion

This method invokes the imageUnfilteredPasteboardTypes() class method and checks the list of types returned by that method against the data types in `pasteboard`. If it finds a match, it returns true. When creating a subclass of `NSImageRep` that accepts image data from a non-default pasteboard type, override the imageUnfilteredPasteboardTypes() method to assure this method returns the correct response.

## See Also

### Determining Types for Images

class func canInit(with: Data) -> Bool

Returns a Boolean value that indicates whether the image representation can initialize itself from the specified data.

class var imageTypes: [String]

Returns an array of UTI strings identifying the image types supported by the image representation, either directly or through a user-installed filter service.

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

