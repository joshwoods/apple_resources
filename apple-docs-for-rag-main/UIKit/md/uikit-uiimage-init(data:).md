

- UIKit
- UIImage
-  init(data:) 

Initializer

# init(data:)

Initializes and returns the image object with the specified data.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(data: Data)
```

## Parameters 

`data`  

The data object containing the image data.

## Return Value

An initialized `UIImage` object, or `nil` if the method could not initialize the image from the specified data.

## Discussion

The data in the `data` parameter must be formatted to match the file format of one of the system’s supported image types.

## See Also

### Creating and initializing image objects

init?(contentsOfFile: String)

Initializes and returns the image object with the contents of the specified file.

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

