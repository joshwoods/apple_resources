

- GameKit
- GKAccessPoint
-  frameInScreenCoordinates 

Instance Property

# frameInScreenCoordinates

The frame of the access point in screen coordinates.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
var frameInScreenCoordinates: CGRect { get }
```

**macOS**

``` source
var frameInScreenCoordinates: NSRect { get }
```

## Mentioned in 

Adding an access point to your game

## Discussion

This is an observable property.

## See Also

### Managing the location

var location: GKAccessPoint.Location

The corner of the screen to display the access point.

enum Location

Specifies the corner of the screen to display the access point.

var parentWindow: UIWindow?

The window that contains the access point.

