

- WatchKit
- WKImage
-  init(image:) 

Initializer

# init(image:)

Creates and returns an image object using the specified UIKit image.

watchOS 2.0+

``` source
convenience init(image: UIImage)
```

## Parameters 

`image`  

The image object. This parameter must not be `nil`.

## Return Value

An initialized `WKImage` object.

## Discussion

Use this method when you already have a UIKit image object and want to use it in your picker.

## See Also

### Creating Image Objects

convenience init(imageData: Data)

Creates an image with the specified raw image data.

convenience init(imageName: String)

Creates an image by loading an image file from the Watch app bundle.

