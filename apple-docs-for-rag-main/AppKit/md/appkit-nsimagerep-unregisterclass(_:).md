

- AppKit
- NSImageRep
-  unregisterClass(\_:) 

Type Method

# unregisterClass(\_:)

Removes the specified image representation subclass from the registry of available image representations.

macOS

``` source
class func unregisterClass(_ imageRepClass: AnyClass)
```

## Parameters 

`imageRepClass`  

The `Class` object for an `NSImageRep` subclass.

## Discussion

This method posts the registryDidChangeNotification, along with the receiving object, to the default notification center.

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

class func `class`(forFileType: String) -> AnyClass?

Returns the image representation subclass that handles data with the specified type.

Deprecated

class func `class`(forPasteboardType: NSPasteboard.PasteboardType) -> AnyClass?

Returns the image representation subclass that handles data with the specified pasteboard type.

Deprecated

