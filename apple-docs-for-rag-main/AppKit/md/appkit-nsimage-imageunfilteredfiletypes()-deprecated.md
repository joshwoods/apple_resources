

- AppKit
- NSImage
-  imageUnfilteredFileTypes() Deprecated

Type Method

# imageUnfilteredFileTypes()

Returns an array of strings identifying the file types supported directly by the registered image representation objects.

macOS 10.0–10.10Deprecated

``` source
class func imageUnfilteredFileTypes() -> [String]
```

Deprecated

Use imageUnfilteredTypes instead.

## Return Value

An array of `NSString` objects, each of which identifies a single supported file type. File types are identified by file extension and HFS file types.

## Discussion

The returned list does not contain pasteboard types that are available only through a user-installed filter service.

## See Also

### Class Methods

class func imageFileTypes() -> [String]

Returns an array of strings identifying the image types supported by the registered image representation objects.

Deprecated

class func imagePasteboardTypes() -> [NSPasteboard.PasteboardType]

Returns an array of strings identifying the pasteboard types supported directly by the registered image representation objects.

Deprecated

class func imageUnfilteredPasteboardTypes() -> [NSPasteboard.PasteboardType]

Returns an array of strings identifying the pasteboard types supported directly by the registered image representation objects.

Deprecated

