

- AppKit
- NSImage
-  imageFileTypes() Deprecated

Type Method

# imageFileTypes()

Returns an array of strings identifying the image types supported by the registered image representation objects.

macOS 10.0–10.10Deprecated

``` source
class func imageFileTypes() -> [String]
```

Deprecated

Use imageTypes instead.

## Return Value

An array of `NSString` objects, each of which identifies a single supported file type. The array can include encoded HFS file types as well as filename extensions.

## Discussion

This list includes all file types supported by registered subclasses of NSImageRep plus those that can be converted to a supported type by a user-installed filter service. You can pass the array returned by this method directly to the runModalForTypes: method of `NSOpenPanel`.

Do not override this method. If your app supports custom image types, create and register an NSImageRep subclass that handles those types.

## See Also

### Class Methods

class func imageUnfilteredFileTypes() -> [String]

Returns an array of strings identifying the file types supported directly by the registered image representation objects.

Deprecated

class func imagePasteboardTypes() -> [NSPasteboard.PasteboardType]

Returns an array of strings identifying the pasteboard types supported directly by the registered image representation objects.

Deprecated

class func imageUnfilteredPasteboardTypes() -> [NSPasteboard.PasteboardType]

Returns an array of strings identifying the pasteboard types supported directly by the registered image representation objects.

Deprecated

