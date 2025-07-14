

- CarPlay
- CPNavigationAlert
-  imageSet 

Instance Property

# imageSet

An image set displayed in the navigation alert.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
@NSCopying
var imageSet: CPImageSet? { get }
```

## Discussion

The navigation alert doesn’t support animated images. If imageSet references an animated image, the alert displays the first image in the animation sequence.

## See Also

### Getting the Alert Image

var image: UIImage?

An image displayed in the navigation alert.

