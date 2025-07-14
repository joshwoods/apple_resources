

- ARKit
- ARGeoAnchor
- ARGeoAnchor.AltitudeSource
-  ARGeoAnchor.AltitudeSource.coarse 

Case

# ARGeoAnchor.AltitudeSource.coarse

The framework sets the altitude using a coarse digital-elevation model.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case coarse
```

## Discussion

The accuracy of this altitude is noticeably imprecise at close range, but it’s sufficient from far away. Use this option to save computational resources for anchors that are far off in the distance.

## See Also

### Sources

case precise

The framework sets the altitude using a high-resolution digital-elevation model.

case userDefined

The app defines the altitude.

case unknown

Altitude isn’t yet set.

