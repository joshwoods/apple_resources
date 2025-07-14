

- Core Image
- CIImage
-  properties 

Instance Property

# properties

A dictionary containing metadata about the image.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
var properties: [String : Any] { get }
```

## Discussion

If the `CIImage` object is the output of a filter (or filter chain), this property’s value is the metadata from the filter’s original input image.

## See Also

### Getting Image Information

var definition: CIFilterShape

Returns a filter shape object that represents the domain of definition of the image.

var extent: CGRect

A rectangle that specifies the extent of the image.

var url: URL?

The URL from which the image was loaded.

var colorSpace: CGColorSpace?

The color space of the image.

func orientationTransform(forExifOrientation: Int32) -> CGAffineTransform

Returns the transformation needed to reorient the image to the specified orientation.

