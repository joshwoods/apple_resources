

- Core Image
- Sharpening Filters
-  unsharpMask() 

Type Method

# unsharpMask()

Increases an image’s contrast between two colors.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class func unsharpMask() -> any CIFilter & CIUnsharpMask
```

## Return Value

The modified image.

## Discussion

This method applies the unsharp mask filter to an image. The effect increases the contrast of the edge between pixels of different colors within the defined radius property.

The unsharp mask filter uses the following properties:

`inputImage`  
An image with the type CIImage.

`radius`  
A `float` representing the area of effect as an NSNumber.

`intensity`  
A `float` representing the desired strength of the effect as an NSNumber.

The following code creates a filter that results in the objects within the image becoming darker:

func unsharp (inputImage: CIImage) -> CIImage? {    
    let unsharpMask = CIFilter.unsharpMask()
    unsharpMask.inputImage = inputImage
    unsharpMask.radius = 5
    unsharpMask.intensity = 2.5
    return unsharpMask.outputImage!
}

## See Also

### Filters

class func sharpenLuminance() -> any CIFilter &amp; CISharpenLuminance

Applies a sharpening effect to an image.

