

- CarPlay
- CPNavigationAlert
-  image 

Instance Property

# image

An image displayed in the navigation alert.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
@NSCopying
var image: UIImage? { get }
```

## Discussion

The navigation alert doesn’t support animated images. If `image` references an animated image, the alert displays first image in the animation sequence.

## See Also

### Getting the Alert Image

var imageSet: CPImageSet?

An image set displayed in the navigation alert.

