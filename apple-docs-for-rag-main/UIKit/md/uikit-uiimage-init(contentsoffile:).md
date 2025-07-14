

- UIKit
- UIImage
-  init(contentsOfFile:) 

Initializer

# init(contentsOfFile:)

Initializes and returns the image object with the contents of the specified file.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(contentsOfFile path: String)
```

## Parameters 

`path`  

The path to the file. This path should include the filename extension that identifies the type of the image data.

## Return Value

An initialized `UIImage` object, or `nil` if the method could not find the file or initialize the image from its contents.

## Discussion

This method loads the image data into memory and marks it as purgeable. If the data is purged and needs to be reloaded, the image object loads that data again from the specified path.

## See Also

### Creating and initializing image objects

init?(data: Data)

Initializes and returns the image object with the specified data.

init?(data: Data, scale: CGFloat)

Initializes and returns the image object with the specified data and scale factor.

init(cgImage: CGImage)

Initializes and returns the image object with the specified Quartz image reference.

init(cgImage: CGImage, scale: CGFloat, orientation: UIImage.Orientation)

Initializes and returns an image object with the specified scale and orientation factors.

init(ciImage: CIImage)

Initializes and returns an image object with the specified Core Image object.

init(ciImage: CIImage, scale: CGFloat, orientation: UIImage.Orientation)

Initializes and returns an image object with the specified Core Image object and properties.

struct UIImageReader

