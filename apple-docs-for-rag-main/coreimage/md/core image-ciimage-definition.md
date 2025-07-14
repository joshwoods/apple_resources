

- Core Image
- CIImage
-  definition 

Instance Property

# definition

Returns a filter shape object that represents the domain of definition of the image.

macOS 10.4+

``` source
var definition: CIFilterShape { get }
```

## Return Value

A filter shape object.

## See Also

### Getting Image Information

var extent: CGRect

A rectangle that specifies the extent of the image.

var properties: [String : Any]

A dictionary containing metadata about the image.

var url: URL?

The URL from which the image was loaded.

var colorSpace: CGColorSpace?

The color space of the image.

func orientationTransform(forExifOrientation: Int32) -> CGAffineTransform

Returns the transformation needed to reorient the image to the specified orientation.

