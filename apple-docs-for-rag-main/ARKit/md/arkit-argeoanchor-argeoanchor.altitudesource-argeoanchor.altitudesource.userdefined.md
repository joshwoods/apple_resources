

- ARKit
- ARGeoAnchor
- ARGeoAnchor.AltitudeSource
-  ARGeoAnchor.AltitudeSource.userDefined 

Case

# ARGeoAnchor.AltitudeSource.userDefined

The app defines the altitude.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case userDefined
```

## Discussion

ARKit records this altitude source when your app defines a geo anchor’s altitude.

You may acquire altitude by providing a particular scene coordinate to the session using getGeoLocation(forPoint:completionHandler:).

For example, your app might set a geo anchor’s altitude by raycasting a surface, then adding an arbitrary `y-`amount to make the anchor more visible from afar.

## See Also

### Sources

case precise

The framework sets the altitude using a high-resolution digital-elevation model.

case coarse

The framework sets the altitude using a coarse digital-elevation model.

case unknown

Altitude isn’t yet set.

