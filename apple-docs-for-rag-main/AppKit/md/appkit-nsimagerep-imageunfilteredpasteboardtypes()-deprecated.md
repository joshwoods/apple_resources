

- AppKit
- NSImageRep
-  imageUnfilteredPasteboardTypes() Deprecated

Type Method

# imageUnfilteredPasteboardTypes()

Returns the list of pasteboard types supported directly by the image representation.

macOS 10.0–10.10Deprecated

``` source
class func imageUnfilteredPasteboardTypes() -> [NSPasteboard.PasteboardType]
```

Deprecated

Use +imageUnfilteredTypes instead

## Return Value

An array of `NSString` objects. This array is empty by default. Subclasses must override to return the list of pasteboard formats they support.

## Discussion

When creating a subclass of `NSImageRep`, override this method to return a list representing the supported pasteboard types. For example, the `NSBitmapImageRep` class implements code similar to the following for this method:

```
+ (NSArray *)imageUnfilteredPasteboardTypes {
    static NSArray *types = nil;

    if (!types) types = [[NSArray alloc] initWithObjects:NSTIFFPboardType,  nil];
    return types;
}
```

If your subclass supports the types supported by its superclass, you must explicitly get the list of types from the superclass and add them to the array returned by this method.

## See Also

### Related Documentation

class func imageUnfilteredPasteboardTypes() -> [NSPasteboard.PasteboardType]

Returns an array of strings identifying the pasteboard types supported directly by the registered image representation objects.

Deprecated

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

class func imagePasteboardTypes() -> [NSPasteboard.PasteboardType]

Returns the pasteboard types supported by the image representation class or one of its subclasses.

Deprecated

class func imageUnfilteredFileTypes() -> [String]

Returns the list of file types supported directly by the image representation.

Deprecated

