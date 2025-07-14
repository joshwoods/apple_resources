

- AVKit
- AVPictureInPictureController
-  pictureInPictureButtonStopImage 

Type Property

# pictureInPictureButtonStopImage

A system-default template image for the button that stops Picture in Picture in your app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
class var pictureInPictureButtonStopImage: UIImage { get }
```

**macOS**

``` source
class var pictureInPictureButtonStopImage: NSImage { get }
```

## Mentioned in 

Adopting Picture in Picture in a Custom Player

## See Also

### Retrieving Picture in Picture Template Images

class var pictureInPictureButtonStartImage: UIImage

A system-default template image for the button that starts Picture in Picture in your app.

class func pictureInPictureButtonStartImage(compatibleWith: UITraitCollection?) -> UIImage

Returns a system-default template image that’s compatible with a trait collection for the button that starts Picture in Picture in your app.

class func pictureInPictureButtonStopImage(compatibleWith: UITraitCollection?) -> UIImage

Returns a system-default template image that’s compatible with a trait collection for the button that stops Picture in Picture in your app.

