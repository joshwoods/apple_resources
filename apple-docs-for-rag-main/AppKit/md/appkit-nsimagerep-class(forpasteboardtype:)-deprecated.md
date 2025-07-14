

- AppKit
- NSImageRep
-  class(forPasteboardType:) Deprecated

Type Method

# class(forPasteboardType:)

Returns the image representation subclass that handles data with the specified pasteboard type.

macOS 10.0–10.10Deprecated

``` source
class func `class`(forPasteboardType type: NSPasteboard.PasteboardType) -> AnyClass?
```

Deprecated

Use +imageRepClassForType: instead

## Parameters 

`type`  

The pasteboard type.

## Return Value

A `Class` object for the image representation that can handle the specified pasteboard type, or `nil` if no image representation could handle the type.

## See Also

### Managing Representation Subclasses of Images

class func `class`(forType: String) -> AnyClass?

Returns the image representation subclass that handles image data for the specified UTI.

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

