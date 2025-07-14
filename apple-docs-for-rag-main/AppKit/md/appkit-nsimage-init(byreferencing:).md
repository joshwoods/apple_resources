

- AppKit
- NSImage
-  init(byReferencing:) 

Initializer

# init(byReferencing:)

Initializes and returns an image object using the specified URL.

macOS

``` source
convenience init(byReferencing url: URL)
```

## Parameters 

`url`  

The URL identifying the image.

## Return Value

An initialized `NSImage` object.

## Discussion

This method initializes the image object lazily. It does not attempt to retrieve the data from the specified URL or create any image representations from that data until an app attempts to draw the image or request information about it.

The `url` parameter should include a file extension that identifies the type of the image data. The mechanism that actually creates the image representation looks for an NSImageRep subclass that handles that data type from among those registered with `NSImage`.

Because this method doesn’t actually create image representations for the image data, your app should do error checking before attempting to use the image; one way to do so is by accessing the isValid property to check whether the image can be drawn.

This method invokes setDataRetained: with an argument of true, thus enabling it to hold onto its URL. When archiving an image created with this method, only the image’s URL is written to the archive.

## See Also

### Creating Images from Resource Files

convenience init?(byReferencingFile: String)

Initializes and returns an image object using the specified file.

convenience init?(contentsOfFile: String)

Initializes and returns an image object with the contents of the specified file.

convenience init?(contentsOf: URL)

Initializes and returns an image object with the contents of the specified URL.

