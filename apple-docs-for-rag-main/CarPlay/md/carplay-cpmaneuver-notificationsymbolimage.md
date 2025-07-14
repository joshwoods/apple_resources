

- CarPlay
- CPManeuver
-  notificationSymbolImage 

Instance Property

# notificationSymbolImage

An image for notification banners that represents the maneuver.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var notificationSymbolImage: UIImage? { get set }
```

## Discussion

You use a named image asset to supply variants for both dark and light interface styles, and initialize the image using init(named:). CarPlay then selects the correct image for the current interface style.

If you don’t provide a notification symbol image, CarPlay uses symbolImage.

## See Also

### Providing symbol images

var symbolImage: UIImage?

An image that represents the maneuver.

var dashboardSymbolImage: UIImage?

An image for the CarPlay dashboard that represents the maneuver.

var symbolSet: CPImageSet?

An image set that represents the maneuver.

Deprecated

