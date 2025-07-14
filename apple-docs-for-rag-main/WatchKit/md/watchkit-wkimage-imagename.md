

- WatchKit
- WKImage
-  imageName 

Instance Property

# imageName

The name of the image to load from the Watch app’s bundle.

watchOS 2.0+

``` source
var imageName: String? { get }
```

## Discussion

The value in this property is set using the init(imageName:) method. For image objects created using other methods, this property is `nil`.

## See Also

### Getting the Image Data

var image: UIImage?

The UIKit image object

var imageData: Data?

The data object containing the raw image data.

