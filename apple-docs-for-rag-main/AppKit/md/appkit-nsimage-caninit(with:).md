

- AppKit
- NSImage
-  canInit(with:) 

Type Method

# canInit(with:)

Tests whether the image can create an instance of itself using pasteboard data.

macOS

``` source
class func canInit(with pasteboard: NSPasteboard) -> Bool
```

## Parameters 

`pasteboard`  

The pasteboard containing the image data.

## Return Value

true if the receiver knows how to handle the data on the pasteboard; otherwise, false.

## Discussion

This method uses the `NSImageRep` class method imageUnfilteredPasteboardTypes() to find a class that can handle the data in the specified pasteboard. If you create your own `NSImageRep` subclasses, override the imageUnfilteredPasteboardTypes() method to notify `NSImage` of the pasteboard types your class supports.

## See Also

### Related Documentation

class func imagePasteboardTypes() -> [NSPasteboard.PasteboardType]

Returns an array of strings identifying the pasteboard types supported directly by the registered image representation objects.

Deprecated

### Determining Supported Types of Images

class var imageTypes: [String]

Returns an array of UTI strings identifying the image types supported by the registered image representation objects, either directly or through a user-installed filter service.

class var imageUnfilteredTypes: [String]

Returns an array of UTI strings identifying the image types supported directly by the registered image representation objects.

