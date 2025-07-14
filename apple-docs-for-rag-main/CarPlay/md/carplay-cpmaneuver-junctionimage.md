

- CarPlay
- CPManeuver
-  junctionImage 

Instance Property

# junctionImage

An image that represents an upcoming junction.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var junctionImage: UIImage? { get set }
```

## Discussion

Provide a junction image to show more visual details about the maneuver, such as the lane a driver should be in when making a turn.

You use a named image asset to supply variants for both dark and light interface styles, and initialize the image using init(named:). CarPlay then selects the correct image for the current interface style.

Note

The maximum image size is 140 x 100 points. CarPlay scales a larger image to fit while maintaining its aspect ratio.

## See Also

### Providing junction images

var dashboardJunctionImage: UIImage?

An image for the CarPlay dashboard that represents an upcoming junction.

