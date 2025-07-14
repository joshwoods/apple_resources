

- AppKit
- NSImageRep
-  registerClass(\_:) 

Type Method

# registerClass(\_:)

Adds the specified class to the registry of available image representation subclasses.

macOS

``` source
class func registerClass(_ imageRepClass: AnyClass)
```

## Parameters 

`imageRepClass`  

The `Class` object for an `NSImageRep` subclass.

## Discussion

This method posts an registryDidChangeNotification, along with the receiving object, to the default notification center.

A good place to add image representation classes to the registry is in the `load` class method.

## See Also

### Related Documentation

class func load()

Invoked whenever a class or category is added to the Objective-C runtime; implement this method to perform class-specific behavior upon loading.

### Managing Representation Subclasses of Images

class func `class`(forType: String) -> AnyClass?

Returns the image representation subclass that handles image data for the specified UTI.

class func `class`(for: Data) -> AnyClass?

Returns the image representation subclass that handles the specified type of data.

class var registeredClasses: [AnyClass]

Returns an array containing the registered image representation classes.

class func unregisterClass(AnyClass)

Removes the specified image representation subclass from the registry of available image representations.

class func `class`(forFileType: String) -> AnyClass?

Returns the image representation subclass that handles data with the specified type.

Deprecated

class func `class`(forPasteboardType: NSPasteboard.PasteboardType) -> AnyClass?

Returns the image representation subclass that handles data with the specified pasteboard type.

Deprecated

