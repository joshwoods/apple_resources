

- Core Image
- CIImage
-  orientationTransform(forExifOrientation:) 

Instance Method

# orientationTransform(forExifOrientation:)

Returns the transformation needed to reorient the image to the specified orientation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func orientationTransform(forExifOrientation orientation: Int32) -> CGAffineTransform
```

## Parameters 

`orientation`  

An integer specifying an image orientation according to the EXIF specification. For details, see kCGImagePropertyOrientation.

## Return Value

An affine transform that will rotate or mirror the image to match the specified orientation when applied.

## Discussion

This method determines the transformation needed to match the specified orientation, but does not apply that transformation to the image. To apply the transformation (possibly after concatenating it with other transformations), use the transformed(by:) method or the `CIAffineTransform` filter. To determine and apply the transformation in a single step, use the oriented(forExifOrientation:) method.

## See Also

### Getting Image Information

var definition: CIFilterShape

Returns a filter shape object that represents the domain of definition of the image.

var extent: CGRect

A rectangle that specifies the extent of the image.

var properties: [String : Any]

A dictionary containing metadata about the image.

var url: URL?

The URL from which the image was loaded.

var colorSpace: CGColorSpace?

The color space of the image.

