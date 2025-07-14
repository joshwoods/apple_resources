

- CarPlay
- CPManeuver
-  symbolImage 

Instance Property

# symbolImage

An image that represents the maneuver.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var symbolImage: UIImage? { get set }
```

## Discussion

You use a named image asset to supply variants for both dark and light interface styles, and initialize the image using init(named:). CarPlay then selects the correct image for the current interface style.

## See Also

### Providing symbol images

var dashboardSymbolImage: UIImage?

An image for the CarPlay dashboard that represents the maneuver.

var notificationSymbolImage: UIImage?

An image for notification banners that represents the maneuver.

var symbolSet: CPImageSet?

An image set that represents the maneuver.

Deprecated

