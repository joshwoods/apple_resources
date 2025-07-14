

- WatchKit
- WKImage
-  imageData 

Instance Property

# imageData

The data object containing the raw image data.

watchOS 2.0+

``` source
var imageData: Data? { get }
```

## Discussion

The value in this property is set using the init(imageData:) method. For image objects created using other methods, this property is `nil`.

## See Also

### Getting the Image Data

var image: UIImage?

The UIKit image object

var imageName: String?

The name of the image to load from the Watch app’s bundle.

