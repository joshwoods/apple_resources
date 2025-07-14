

- UIKit
- UIImage
-  init(cgImage:) 

Initializer

# init(cgImage:)

Initializes and returns the image object with the specified Quartz image reference.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(cgImage: CGImage)
```

## Parameters 

`cgImage`  

A Quartz image reference.

## Return Value

An initialized `UIImage` object, or `nil` if the method could not initialize the image from the specified data.

## See Also

### Creating and initializing image objects

init?(contentsOfFile: String)

Initializes and returns the image object with the contents of the specified file.

init?(data: Data)

Initializes and returns the image object with the specified data.

init?(data: Data, scale: CGFloat)

Initializes and returns the image object with the specified data and scale factor.

init(cgImage: CGImage, scale: CGFloat, orientation: UIImage.Orientation)

Initializes and returns an image object with the specified scale and orientation factors.

init(ciImage: CIImage)

Initializes and returns an image object with the specified Core Image object.

init(ciImage: CIImage, scale: CGFloat, orientation: UIImage.Orientation)

Initializes and returns an image object with the specified Core Image object and properties.

struct UIImageReader

