

- Core Image
- CIImage
-  clampedToExtent() 

Instance Method

# clampedToExtent()

Returns a new image created by making the pixel colors along its edges extend infinitely in all directions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func clampedToExtent() -> CIImage
```

## Return Value

An image object representing the result of the clamp operation.

## Discussion

Calling this method is equivalent to using the CIAffineClamp filter, which creates an image of infinite extent by repeating pixel colors from the edges of the original image.

This operation can be useful when using the image as input to other filters. When an image has finite extent, Core Image treats the area outside the extent as if it were filled with empty (black, zero alpha) pixels. If you apply a filter that samples from outside the image’s extent, those empty pixels affect the result of the filter.

For example, applying the `CIGaussianBlur` filter to an image softens the edges of the blurred image, because the opaque pixels at the edges of the image blur into the transparent pixels outside the image’s extent. Applying a clamp effect before the blur filter avoids edge softening by making the original image opaque in all directions. (However, the blurred image will also have infinite extent. Use the cropped(to:) method to return to the original image’s dimensions while retaining hard edges.)

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

func oriented(forExifOrientation: Int32) -> CIImage

Returns a new image created by transforming the original image to the specified EXIF orientation.

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

