

- AppKit
- NSImageRep
-  init(contentsOfFile:) 

Initializer

# init(contentsOfFile:)

Creates and returns an image representation object using the contents of the specified file.

macOS

``` source
init?(contentsOfFile filename: String)
```

## Parameters 

`filename`  

A full or relative pathname specifying the file to open. This string should include the filename extension.

## Return Value

An initialized instance of an `NSImageRep` subclass, or `nil` if the image data could not be read.

## Discussion

If sent to the `NSImageRep` class object, this method returns a newly allocated instance of a subclass of `NSImageRep` (chosen through the use of class(forFileType:)) initialized with the contents of the specified file. If sent to a subclass of `NSImageRep` that recognizes the type of data in the file, it returns an instance of that subclass initialized with the contents of the file.

This method returns `nil` in any of the following cases:

- The message is sent to the `NSImageRep` class object and there are no subclasses in the `NSImageRep` class registry that handle the type of data in the specified file.

- The message is sent to a subclass of `NSImageRep` and that subclass cannot handle the type of data in the specified file.

- The `NSImageRep` subclass is unable to initialize itself with the contents of the specified file.

The `NSImageRep` subclass is initialized by creating an `NSData` object based on the contents of the file and passing it to the `imageRepWithData:` method. By default, the files handled include those with the extensions “`tiff`”, “`gif`”, “`jpg`”, “`pict`”, “`pdf`”, and “`eps`”.

## See Also

### Related Documentation

class func imageFileTypes() -> [String]

Returns the file types supported by the image representation class or one of its subclasses.

Deprecated

### Creating Representations of Images

class func imageReps(withContentsOfFile: String) -> [NSImageRep]?

Creates and returns an array of image representation objects initialized using the contents of the specified file.

class func imageReps(with: NSPasteboard) -> [NSImageRep]?

Creates and returns an array of image representation objects initialized using the contents of the pasteboard.

class func imageReps(withContentsOf: URL) -> [NSImageRep]?

Creates and returns an array of image representation objects initialized using the contents of the specified URL.

init?(pasteboard: NSPasteboard)

Creates and returns an image representation object using the contents of the specified pasteboard.

init?(contentsOf: URL)

Creates and returns an image representation object using the data at the specified URL.

init()

Creates and returns an image representation object.

init?(coder: NSCoder)

Creates and returns an image representation object from data in an unarchiver.

