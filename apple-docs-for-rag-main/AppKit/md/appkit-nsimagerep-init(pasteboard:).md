

- AppKit
- NSImageRep
-  init(pasteboard:) 

Initializer

# init(pasteboard:)

Creates and returns an image representation object using the contents of the specified pasteboard.

macOS

``` source
init?(pasteboard: NSPasteboard)
```

## Parameters 

`pasteboard`  

The pasteboard containing the image data.

## Return Value

An initialized instance of an `NSImageRep` subclass, or `nil` if the image data could not be read.

## Discussion

If sent to the `NSImageRep` class object, this method returns a newly allocated instance of a subclass of `NSImageRep` initialized with the data in the specified pasteboard. If sent to a subclass of `NSImageRep` that recognizes the data on the pasteboard, it returns an instance of that subclass initialized with that data.

This method returns `nil` in any of the following cases:

- The message is sent to the `NSImageRep` class object and there are no subclasses in the `NSImageRep` class registry that handle data of the type contained in the specified pasteboard.

- The message is sent to a subclass of `NSImageRep` and that subclass cannot handle data of the type contained in the specified pasteboard.

- The `NSImageRep` subclass is unable to initialize itself with the contents of the pasteboard.

The `NSImageRep` subclass is initialized by creating an `NSData` object based on the data the specified pasteboard and passing it to the `imageRepWithData:` method.

## See Also

### Related Documentation

class func imagePasteboardTypes() -> [NSPasteboard.PasteboardType]

Returns the pasteboard types supported by the image representation class or one of its subclasses.

Deprecated

### Creating Representations of Images

class func imageReps(withContentsOfFile: String) -> [NSImageRep]?

Creates and returns an array of image representation objects initialized using the contents of the specified file.

class func imageReps(with: NSPasteboard) -> [NSImageRep]?

Creates and returns an array of image representation objects initialized using the contents of the pasteboard.

class func imageReps(withContentsOf: URL) -> [NSImageRep]?

Creates and returns an array of image representation objects initialized using the contents of the specified URL.

init?(contentsOfFile: String)

Creates and returns an image representation object using the contents of the specified file.

init?(contentsOf: URL)

Creates and returns an image representation object using the data at the specified URL.

init()

Creates and returns an image representation object.

init?(coder: NSCoder)

Creates and returns an image representation object from data in an unarchiver.

