

- Core Image
- CIImage
-  oriented(forExifOrientation:) 

Instance Method

# oriented(forExifOrientation:)

Returns a new image created by transforming the original image to the specified EXIF orientation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func oriented(forExifOrientation orientation: Int32) -> CIImage
```

## Parameters 

`orientation`  

An integer specifying an image orientation according to the EXIF specification. For details, see kCGImagePropertyOrientation.

## Return Value

An image object representing the result of rotating or mirroring the image to the target orientation.

## Discussion

This method determines and then applies the transformation needed to reorient the image to the specified orientation. If you plan to also apply other transformations, you can retrieve the transformation this method would use by calling the orientationTransform(forExifOrientation:) method.

## See Also

### Creating an Image by Modifying an Existing Image

func applyingFilter(String, parameters: [String : Any]) -> CIImage

Returns a new image created by applying a filter to the original image with the specified name and parameters.

func applyingFilter(String) -> CIImage

Applies the filter to an image and returns the output.

func transformed(by: CGAffineTransform) -> CIImage

Returns a new image that represents the original image after applying an affine transform.

func transformed(by: CGAffineTransform, highQualityDownsample: Bool) -> CIImage

func cropped(to: CGRect) -> CIImage

Returns a new image with a cropped portion of the original image.

func clampedToExtent() -> CIImage

Returns a new image created by making the pixel colors along its edges extend infinitely in all directions.

func clamped(to: CGRect) -> CIImage

Returns a new image created by cropping to a specified area, then making the pixel colors along the edges of the cropped image extend infinitely in all directions.

func composited(over: CIImage) -> CIImage

Returns a new image created by compositing the original image over the specified destination image.

func convertingWorkingSpaceToLab() -> CIImage

func convertingLabToWorkingSpace() -> CIImage

func matchedToWorkingSpace(from: CGColorSpace) -> CIImage?

Returns a new image created by color matching from the specified color space to the context’s working color space.

func matchedFromWorkingSpace(to: CGColorSpace) -> CIImage?

Returns a new image created by color matching from the context’s working color space to the specified color space.

func premultiplyingAlpha() -> CIImage

Returns a new image created by multiplying the image’s RGB values by its alpha values.

func unpremultiplyingAlpha() -> CIImage

Returns a new image created by dividing the image’s RGB values by its alpha values.

func settingAlphaOne(in: CGRect) -> CIImage

Returns a new image created by setting all alpha values to 1.0 within the specified rectangle and to 0.0 outside of that area.

func applyingGaussianBlur(sigma: Double) -> CIImage

Returns a new image created by applying a Gaussian Blur filter to the image.

func settingProperties([AnyHashable : Any]) -> CIImage

Returns a new image created by adding the specified metadata properties to the image.

func insertingIntermediate() -> CIImage

Returns a new image created by inserting an intermediate.

func insertingIntermediate(cache: Bool) -> CIImage

Returns a new image created by inserting a cacheable intermediate.

