

- CarPlay
- CPBarButton
-  image 

Instance Property

# image

The image displayed on the bar button.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var image: UIImage? { get set }
```

## Discussion

If you provide an animated image, the button displays only the first image in the animation sequence.

Setting this property has an effect only when the button type is CPBarButton.Type.image.

## See Also

### Configuring the Button

var isEnabled: Bool

A Boolean value that enables and disables the bar button.

var title: String?

The title displayed on the bar button.

