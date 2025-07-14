

- AVKit
- AVPictureInPictureController
-  pictureInPictureButtonStartImage(compatibleWith:) 

Type Method

# pictureInPictureButtonStartImage(compatibleWith:)

Returns a system-default template image that’s compatible with a trait collection for the button that starts Picture in Picture in your app.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
class func pictureInPictureButtonStartImage(compatibleWith traitCollection: UITraitCollection?) -> UIImage
```

## Parameters 

`traitCollection`  

A trait collection that describes the image to retrieve. Pass `nil` to use traits that describe the main screen.

## Return Value

A system-default template image.

## See Also

### Retrieving Picture in Picture Template Images

class var pictureInPictureButtonStartImage: UIImage

A system-default template image for the button that starts Picture in Picture in your app.

class var pictureInPictureButtonStopImage: UIImage

A system-default template image for the button that stops Picture in Picture in your app.

class func pictureInPictureButtonStopImage(compatibleWith: UITraitCollection?) -> UIImage

Returns a system-default template image that’s compatible with a trait collection for the button that stops Picture in Picture in your app.

