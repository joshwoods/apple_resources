

- CarPlay
- CPMapButton
-  focusedImage 

Instance Property

# focusedImage

The image to display when focus is on the button.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var focusedImage: UIImage? { get set }
```

## Discussion

If `focusedImage` is nil, the button uses image as the default, creating a focused image using the alpha values from the image.

## See Also

### Providing Button Images

var image: UIImage?

The image to display on the button.

