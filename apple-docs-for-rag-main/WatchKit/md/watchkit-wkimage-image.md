

- WatchKit
- WKImage
-  image 

Instance Property

# image

The UIKit image object

watchOS 2.0+

``` source
var image: UIImage? { get }
```

## Discussion

The value in this property is set using the init(image:) method. For image objects created using other methods, this property is `nil`.

## See Also

### Getting the Image Data

var imageData: Data?

The data object containing the raw image data.

var imageName: String?

The name of the image to load from the Watch app’s bundle.

