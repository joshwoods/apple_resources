

- UIKit
- UIImage
-  init(data:scale:) 

Initializer

# init(data:scale:)

Initializes and returns the image object with the specified data and scale factor.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(
    data: Data,
    scale: CGFloat
)
```

## Parameters 

`data`  

The data object containing the image data.

`scale`  

The scale factor to assume when interpreting the image data. Applying a scale factor of 1.0 results in an image whose size matches the pixel-based dimensions of the image. Applying a different scale factor changes the size of the image as reported by the size property.

## Return Value

An initialized `UIImage` object, or `nil` if the method could not initialize the image from the specified data.

## Discussion

The data in the `data` parameter must be formatted to match the file format of one of the system’s supported image types.

## See Also

### Creating and initializing image objects

init?(contentsOfFile: String)

Initializes and returns the image object with the contents of the specified file.

init?(data: Data)

Initializes and returns the image object with the specified data.

init(cgImage: CGImage)

Initializes and returns the image object with the specified Quartz image reference.

init(cgImage: CGImage, scale: CGFloat, orientation: UIImage.Orientation)

Initializes and returns an image object with the specified scale and orientation factors.

init(ciImage: CIImage)

Initializes and returns an image object with the specified Core Image object.

init(ciImage: CIImage, scale: CGFloat, orientation: UIImage.Orientation)

Initializes and returns an image object with the specified Core Image object and properties.

struct UIImageReader

