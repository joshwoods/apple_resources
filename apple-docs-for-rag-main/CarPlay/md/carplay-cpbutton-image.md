

- CarPlay
- CPButton
-  image 

Instance Property

# image

The button’s image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
@NSCopying
var image: UIImage? { get }
```

## Discussion

This property returns the custom image you provide at initialization, or a system image when using a concrete subclass like CPContactCallButton.

CarPlay doesn’t support animated images. If you provide an animated image, this property returns the first image in the animation sequence.

