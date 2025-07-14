

- Core Image
- CIImage
-  url 

Instance Property

# url

The URL from which the image was loaded.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
var url: URL? { get }
```

## Discussion

A URL is available only if the image object was created with a URL (such as with the init(contentsOf:) method or related methods). Otherwise, this property’s value is `nil`.

## See Also

### Getting Image Information

var definition: CIFilterShape

Returns a filter shape object that represents the domain of definition of the image.

var extent: CGRect

A rectangle that specifies the extent of the image.

var properties: [String : Any]

A dictionary containing metadata about the image.

var colorSpace: CGColorSpace?

The color space of the image.

func orientationTransform(forExifOrientation: Int32) -> CGAffineTransform

Returns the transformation needed to reorient the image to the specified orientation.

