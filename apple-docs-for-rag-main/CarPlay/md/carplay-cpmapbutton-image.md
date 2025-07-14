

- CarPlay
- CPMapButton
-  image 

Instance Property

# image

The image to display on the button.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var image: UIImage? { get set }
```

## Discussion

This property doesn’t support animated images. If it’s set with an animated image, the button displays the first image in the animated sequence.

## See Also

### Providing Button Images

var focusedImage: UIImage?

The image to display when focus is on the button.

