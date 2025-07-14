

- AppKit
- NSImageRep
-  init(coder:) 

Initializer

# init(coder:)

Creates and returns an image representation object from data in an unarchiver.

macOS

``` source
init?(coder: NSCoder)
```

## See Also

### Creating Representations of Images

class func imageReps(withContentsOfFile: String) -> [NSImageRep]?

Creates and returns an array of image representation objects initialized using the contents of the specified file.

class func imageReps(with: NSPasteboard) -> [NSImageRep]?

Creates and returns an array of image representation objects initialized using the contents of the pasteboard.

class func imageReps(withContentsOf: URL) -> [NSImageRep]?

Creates and returns an array of image representation objects initialized using the contents of the specified URL.

init?(contentsOfFile: String)

Creates and returns an image representation object using the contents of the specified file.

init?(pasteboard: NSPasteboard)

Creates and returns an image representation object using the contents of the specified pasteboard.

init?(contentsOf: URL)

Creates and returns an image representation object using the data at the specified URL.

init()

Creates and returns an image representation object.

