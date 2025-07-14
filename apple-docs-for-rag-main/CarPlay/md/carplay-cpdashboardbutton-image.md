

- CarPlay
- CPDashboardButton
-  image 

Instance Property

# image

The image the button displays.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
var image: UIImage { get }
```

## Discussion

CarPlays doesn’t support animated images. If you provide an animated image, the button displays only the first image in the animation sequence. The maximum supported image size is 30 x 30 points.

## See Also

### Accessing the Button Configuration

var titleVariants: [String]

The array of title variants for the button.

var subtitleVariants: [String]

The array of subtitle variants for the button.

