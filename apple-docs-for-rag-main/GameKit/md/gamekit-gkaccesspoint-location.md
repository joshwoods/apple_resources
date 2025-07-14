

- GameKit
- GKAccessPoint
-  location 

Instance Property

# location

The corner of the screen to display the access point.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var location: GKAccessPoint.Location { get set }
```

## Mentioned in 

Adding an access point to your game

## Discussion

Use this property to set one of four corners to display the access point in your game. The default for left-to-right languages is the upper-left corner, and for right-to-left languages, it’s the upper-right corner.

If the parentWindow property is `nil` for volumetric and immersive visionOS games, GameKit doesn’t use the location property. For more information, see Configure the access point on visionOS.

## See Also

### Managing the location

enum Location

Specifies the corner of the screen to display the access point.

var frameInScreenCoordinates: CGRect

The frame of the access point in screen coordinates.

var parentWindow: UIWindow?

The window that contains the access point.

