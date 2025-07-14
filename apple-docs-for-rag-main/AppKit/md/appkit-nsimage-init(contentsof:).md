

- AppKit
- NSImage
-  init(contentsOf:) 

Initializer

# init(contentsOf:)

Initializes and returns an image object with the contents of the specified URL.

macOS

``` source
convenience init?(contentsOf url: URL)
```

## Parameters 

`url`  

The URL identifying the image.

## Return Value

An initialized `NSImage` object or `nil` if the method cannot create an image representation from the contents of the specified URL.

## See Also

### Creating Images from Resource Files

convenience init?(byReferencingFile: String)

Initializes and returns an image object using the specified file.

convenience init(byReferencing: URL)

Initializes and returns an image object using the specified URL.

convenience init?(contentsOfFile: String)

Initializes and returns an image object with the contents of the specified file.

