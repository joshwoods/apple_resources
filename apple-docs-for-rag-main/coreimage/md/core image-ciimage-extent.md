

- Core Image
- CIImage
-  extent 

Instance Property

# extent

A rectangle that specifies the extent of the image.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
var extent: CGRect { get }
```

## Discussion

This rectangle specifies the extent of the image in working space coordinates.

## See Also

### Getting Image Information

var definition: CIFilterShape

Returns a filter shape object that represents the domain of definition of the image.

var properties: [String : Any]

A dictionary containing metadata about the image.

var url: URL?

The URL from which the image was loaded.

var colorSpace: CGColorSpace?

The color space of the image.

func orientationTransform(forExifOrientation: Int32) -> CGAffineTransform

Returns the transformation needed to reorient the image to the specified orientation.

