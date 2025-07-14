

- WatchKit
- WKImage
-  init(imageName:) 

Initializer

# init(imageName:)

Creates an image by loading an image file from the Watch app bundle.

watchOS 2.0+

``` source
convenience init(imageName: String)
```

## Parameters 

`imageName`  

The name of the image to be loaded from the Watch app’s bundle. Specify the filename of the image and include the filename extension in the name. This parameter must not be `nil`.

## Return Value

An initialized `WKImage` object.

## Discussion

Use this method to specify an image by name. Only the image name is sent from your WatchKit extension to your Watch app, and the Watch app handles the loading of that image from its own bundle. If it cannot find the specified image, it displays no image.

## See Also

### Creating Image Objects

convenience init(image: UIImage)

Creates and returns an image object using the specified UIKit image.

convenience init(imageData: Data)

Creates an image with the specified raw image data.

