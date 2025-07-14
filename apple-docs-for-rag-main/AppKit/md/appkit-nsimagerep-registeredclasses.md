

- AppKit
- NSImageRep
-  registeredClasses 

Type Property

# registeredClasses

Returns an array containing the registered image representation classes.

macOS

``` source
class var registeredClasses: [AnyClass] { get }
```

## Return Value

An array of `Class` objects identifying the registered `NSImageRep` subclasses.

## See Also

### Managing Representation Subclasses of Images

class func `class`(forType: String) -> AnyClass?

Returns the image representation subclass that handles image data for the specified UTI.

class func `class`(for: Data) -> AnyClass?

Returns the image representation subclass that handles the specified type of data.

class func registerClass(AnyClass)

Adds the specified class to the registry of available image representation subclasses.

class func unregisterClass(AnyClass)

Removes the specified image representation subclass from the registry of available image representations.

class func `class`(forFileType: String) -> AnyClass?

Returns the image representation subclass that handles data with the specified type.

Deprecated

class func `class`(forPasteboardType: NSPasteboard.PasteboardType) -> AnyClass?

Returns the image representation subclass that handles data with the specified pasteboard type.

Deprecated

