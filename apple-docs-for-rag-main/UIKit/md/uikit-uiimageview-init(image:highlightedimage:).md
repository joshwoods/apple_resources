

- UIKit
- UIImageView
-  init(image:highlightedImage:) 

Initializer

# init(image:highlightedImage:)

Returns an image view initialized with the specified regular and highlighted images.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(
    image: UIImage?,
    highlightedImage: UIImage?
)
```

## Parameters 

`image`  

The initial image to display in the image view. You may specify an image object that contains an animated sequence of images.

`highlightedImage`  

The image to display when the image view is highlighted. You may specify an image object that contains an animated sequence of images.

## Return Value

An initialized image view object.

## Discussion

The images you specify are used to configure the initial size of the image view itself. Use constraints and the image view’s content mode to adjust the image view’s final size onscreen. This method disables user interactions for the image view by setting the isUserInteractionEnabled property to false.

If you specify an animated image whose duration is greater than `0`, the image view automatically starts playing the animation.

## See Also

### Creating an image view

init(image: UIImage?)

Returns an image view initialized with the specified image.

