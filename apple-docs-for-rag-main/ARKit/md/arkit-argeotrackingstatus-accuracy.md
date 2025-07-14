

- ARKit
- ARGeoTrackingStatus
-  accuracy 

Instance Property

# accuracy

The accuracy of geo tracking at the time the session captured the frame.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var accuracy: ARGeoTrackingStatus.Accuracy { get }
```

## Discussion

ARKit populates this property after reaching ARGeoTrackingStatus.State.localized. To ensure the best possible user experience, an app must monitor and react to the geo-tracking accuracy. For more information, see ARGeoTrackingStatus.Accuracy.

## See Also

### Judging Accuracy

enum Accuracy

Values that are possible for the current accuracy of geo tracking.

