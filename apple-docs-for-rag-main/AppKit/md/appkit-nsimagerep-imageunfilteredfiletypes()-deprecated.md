

- AppKit
- NSImageRep
-  imageUnfilteredFileTypes() Deprecated

Type Method

# imageUnfilteredFileTypes()

Returns the list of file types supported directly by the image representation.

macOS 10.0–10.10Deprecated

``` source
class func imageUnfilteredFileTypes() -> [String]
```

Deprecated

Use +imageUnfilteredTypes instead

## Return Value

An array of `NSString` objects. This array is empty by default. Subclasses must override to return the list of file formats they support.

## Discussion

The returned file types can include encoded HFS file types as well as filename extensions. When creating a subclass of `NSImageRep`, override this method to return a list of strings representing the supported file types. For example, the `NSBitmapImageRep` class implements code similar to the following for this method:

```
+ (NSArray *)imageUnfilteredFileTypes {
    static NSArray *types = nil;

    if (!types) types = [[NSArray alloc]
        initWithObjects:@"tiff", @"gif", @"jpg",  @"bmp", nil];
    return types;
}
```

If your subclass supports the types supported by its superclass, you must explicitly get the array of types from the superclass and put them in the array returned by this method.

## See Also

### Related Documentation

class func imageUnfilteredFileTypes() -> [String]

Returns an array of strings identifying the file types supported directly by the registered image representation objects.

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

class func imageUnfilteredPasteboardTypes() -> [NSPasteboard.PasteboardType]

Returns the list of pasteboard types supported directly by the image representation.

Deprecated

