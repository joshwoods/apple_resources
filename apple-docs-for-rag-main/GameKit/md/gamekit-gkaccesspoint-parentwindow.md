

- GameKit
- GKAccessPoint
-  parentWindow 

Instance Property

# parentWindow

The window that contains the access point.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

**macOS**

``` source
weak var parentWindow: NSWindow? { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
weak var parentWindow: UIWindow? { get set }
```

## Mentioned in 

Adding an access point to your game

## Discussion

For Mac games, use this property to specify the parent window of the access point. If you don’t specify a parent widow, GameKit tries to add the access point to the app’s main window. For iPadOS and iOS games, and for compatible iPad or iPhone games running in visionOS, GameKit adds the access point to the main window.

If this property is `nil` for a volumetric visionOS game, the access point doesn’t appear. For an immersive game, it appears below the HUD in front of the person and tracks their head position. If this property is non-`nil` for a volumetric or immersive game, the access point appears outside of the window in the specified location. For more information, see Configure the access point on visionOS.

## See Also

### Managing the location

var location: GKAccessPoint.Location

The corner of the screen to display the access point.

enum Location

Specifies the corner of the screen to display the access point.

var frameInScreenCoordinates: CGRect

The frame of the access point in screen coordinates.

