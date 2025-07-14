

- Core Image
- Sharpening Filters
-  sharpenLuminance() 

Type Method

# sharpenLuminance()

Applies a sharpening effect to an image.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func sharpenLuminance() -> any CIFilter & CISharpenLuminance
```

## Return Value

The modified image.

## Discussion

This method applies the sharpen luminance filter to an image. The effect increases image detail by adjusting the luminance of each pixel within the `radius` property. Sharpening the luminance doesn’t effect the chroma data of each pixel.

The bicubic sharpen luminance filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`radius`  
A `float` representing the area of effect as an NSNumber.

`sharpness`  
A `float` representing the desired strength of the effect as an NSNumber.

The following code creates a filter that results in detail from the sign in the image to be more visible:

func sharpen (inputImage: CIImage) -> CIImage? {
    let sharpenLuminance = CIFilter.sharpenLuminance()
    sharpenLuminance.inputImage = inputImage
    sharpenLuminance.radius = 10
    sharpenLuminance.sharpness = 1
    return sharpenLuminance.outputImage!
}

## See Also

### Filters

class func unsharpMask() -> any CIFilter &amp; CIUnsharpMask

Increases an image’s contrast between two colors.

