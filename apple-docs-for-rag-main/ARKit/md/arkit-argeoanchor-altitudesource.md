

- ARKit
- ARGeoAnchor
-  altitudeSource 

Instance Property

# altitudeSource

A record of the source from which an altitude came.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var altitudeSource: ARGeoAnchor.AltitudeSource { get }
```

## Discussion

The value of this property is ARGeoAnchor.AltitudeSource.userDefined if you set the altitude yourself (see getGeoLocation(forPoint:completionHandler:)).

If your app doesn’t set the altitude, ARKit populates this property to indicate the altitude’s expected accuracy (either ARGeoAnchor.AltitudeSource.precise, or ARGeoAnchor.AltitudeSource.coarse), depending on the level of confidence ARKit has with the altitude data that’s available at the time.

## See Also

### Defining Altitude

var altitude: CLLocationDistance?

Vertical distance, in meters, between this anchor and sea level.

enum AltitudeSource

Options for setting a location anchor’s altitude.

