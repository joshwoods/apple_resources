

- AppKit
- NSImageRep
-  class(forType:) 

Type Method

# class(forType:)

Returns the image representation subclass that handles image data for the specified UTI.

macOS 10.5+

``` source
class func `class`(forType type: String) -> AnyClass?
```

## Parameters 

`type`  

The UTI string identifying the desired image type. Some sample image-related UTI strings include “`public.image`”, “`public.jpeg`”, and “`public.tiff`”. For a list of supported types, see `UTCoreTypes.h`.

## Return Value

A `Class` object for the image representation that can handle the UTI, or `nil` if no image representation could handle the data.

## See Also

### Managing Representation Subclasses of Images

class func `class`(for: Data) -> AnyClass?

Returns the image representation subclass that handles the specified type of data.

class var registeredClasses: [AnyClass]

Returns an array containing the registered image representation classes.

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

