

- WebKit
- WebPreferences
-  allowsAnimatedImageLooping Deprecated

Instance Property

# allowsAnimatedImageLooping

A Boolean that indicates whether or not the receiver allows animated images to loop.

macOS 10.3–10.14Deprecated

``` source
var allowsAnimatedImageLooping: Bool { get set }
```

## Discussion

true if the web view should loop animated images, false otherwise.

If image looping is disabled, the web view displays it as a static image. The number of times that an image loops is determined by parameters of the image file itself and cannot be set in the web view.

## See Also

### Handling Images

var allowsAnimatedImages: Bool

A Boolean that indicates whether or not the receiver allows animated images.

Deprecated

var loadsImagesAutomatically: Bool

A Boolean that indicates whether or not the web view allows images to be loaded automatically.

Deprecated

