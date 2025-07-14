

- UIKit
- UIImage
-  init(cgImage:scale:orientation:) 

Initializer

# init(cgImage:scale:orientation:)

Initializes and returns an image object with the specified scale and orientation factors.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(
    cgImage: CGImage,
    scale: CGFloat,
    orientation: UIImage.Orientation
)
```

## Parameters 

`cgImage`  

The Quartz image object.

`scale`  

The scale factor to assume when interpreting the image data. Applying a scale factor of 1.0 results in an image whose size matches the pixel-based dimensions of the image. Applying a different scale factor changes the size of the image as reported by the size property.

`orientation`  

The orientation of the image data. You can use this parameter to specify any rotation factors applied to the image.

## Return Value

An initialized `UIImage` object. In Objective-C, this method returns `nil` if the `ciImage` parameter is `nil`.

## See Also

### Creating and initializing image objects

init?(contentsOfFile: String)

Initializes and returns the image object with the contents of the specified file.

init?(data: Data)

Initializes and returns the image object with the specified data.

init?(data: Data, scale: CGFloat)

Initializes and returns the image object with the specified data and scale factor.

init(cgImage: CGImage)

Initializes and returns the image object with the specified Quartz image reference.

init(ciImage: CIImage)

Initializes and returns an image object with the specified Core Image object.

init(ciImage: CIImage, scale: CGFloat, orientation: UIImage.Orientation)

Initializes and returns an image object with the specified Core Image object and properties.

struct UIImageReader

