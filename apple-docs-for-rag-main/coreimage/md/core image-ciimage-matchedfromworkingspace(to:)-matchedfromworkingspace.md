

- Core Image
- CIImage
-  matchedFromWorkingSpace(to:) 

Instance Method

# matchedFromWorkingSpace(to:)

Returns a new image created by color matching from the context’s working color space to the specified color space.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func matchedFromWorkingSpace(to colorSpace: CGColorSpace) -> CIImage?
```

## Parameters 

`colorSpace`  

The color space to be converted to. This color space must conform to the CGColorSpaceModel.rgb color space model.

## Return Value

An image object representing the result of the color matching operation, or `nil` if the color spaces to be converted are not compatible.

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

