

- CarPlay
- CPNowPlayingImageButton
-  image 

Instance Property

# image

The image that the button displays.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var image: UIImage? { get }
```

## Discussion

The button displays images no larger than CPNowPlayingButtonMaximumImageSize. If you use an animated image, this property returns the first image in the animation sequence.

