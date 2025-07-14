

- ARKit
- ARFrame
-  geoTrackingStatus 

Instance Property

# geoTrackingStatus

The session’s condition with respect to geographic tracking at the time the session captured the frame.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var geoTrackingStatus: ARGeoTrackingStatus? { get }
```

## Discussion

For the current geo-tracking status, check the value of this property on the session’s currentFrame. ARKit populates this property only for ARGeoTrackingConfiguration sessions.

## See Also

### Assessing geo-tracking condition

class ARGeoTrackingStatus

The state, accuracy, and reason that are possible for geo-tracking’s current condition.

