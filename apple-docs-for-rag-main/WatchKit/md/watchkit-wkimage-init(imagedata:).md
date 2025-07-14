

- WatchKit
- WKImage
-  init(imageData:) 

Initializer

# init(imageData:)

Creates an image with the specified raw image data.

watchOS 2.0+

``` source
convenience init(imageData: Data)
```

## Parameters 

`imageData`  

A data object containing the image data in its native format. This parameter must not be `nil`.

## Return Value

An initialized `WKImage` object.

## Discussion

Use this method when you already have raw PNG or JPG data and want to use it for an image. Using this method for raw image data is more efficient than creating an image object to encapsulate that data.

## See Also

### Creating Image Objects

convenience init(image: UIImage)

Creates and returns an image object using the specified UIKit image.

convenience init(imageName: String)

Creates an image by loading an image file from the Watch app bundle.

