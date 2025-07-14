

- AppKit
- NSImage
-  init(contentsOfFile:) 

Initializer

# init(contentsOfFile:)

Initializes and returns an image object with the contents of the specified file.

macOS

``` source
convenience init?(contentsOfFile fileName: String)
```

## Parameters 

`fileName`  

A full or relative path name specifying the file with the desired image data. Relative paths must be relative to the current working directory.

## Return Value

An initialized `NSImage` object or `nil` if the method cannot create an image representation from the contents of the specified file.

## Discussion

Unlike init(byReferencingFile:), which initializes an `NSImage` object lazily, this method immediately opens the specified file and creates one or more image representations from its data.

The `filename` parameter should include the file extension that identifies the type of the image data. This method looks for an `NSImageRep` subclass that handles that data type from among those registered with `NSImage`.

## See Also

### Creating Images from Resource Files

convenience init?(byReferencingFile: String)

Initializes and returns an image object using the specified file.

convenience init(byReferencing: URL)

Initializes and returns an image object using the specified URL.

convenience init?(contentsOf: URL)

Initializes and returns an image object with the contents of the specified URL.

