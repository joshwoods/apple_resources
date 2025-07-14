

- AppKit
- NSImage
-  imagePasteboardTypes() Deprecated

Type Method

# imagePasteboardTypes()

Returns an array of strings identifying the pasteboard types supported directly by the registered image representation objects.

macOS 10.0–10.10Deprecated

``` source
class func imagePasteboardTypes() -> [NSPasteboard.PasteboardType]
```

Deprecated

Use +imageTypes instead

## Return Value

An array of `NSString` objects, each of which identifies a single supported pasteboard type. By default, this list contains the `NSPDFPboardType`, `NSPICTPboardType`, `NSPostScriptPboardType`, and `NSTIFFPboardType` types.

## Discussion

This list includes all pasteboard types supported by registered subclasses of NSImageRep plus those that can be converted to a supported type by a user-installed filter service.

Do not override this method. Instead, override the imageUnfilteredPasteboardTypes() method to notify `NSImage` of the pasteboard types your class supports.

## See Also

### Class Methods

class func imageFileTypes() -> [String]

Returns an array of strings identifying the image types supported by the registered image representation objects.

Deprecated

class func imageUnfilteredFileTypes() -> [String]

Returns an array of strings identifying the file types supported directly by the registered image representation objects.

Deprecated

class func imageUnfilteredPasteboardTypes() -> [NSPasteboard.PasteboardType]

Returns an array of strings identifying the pasteboard types supported directly by the registered image representation objects.

Deprecated

