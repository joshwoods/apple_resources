

- ARKit
- ARGeoTrackingStatus
- ARGeoTrackingStatus.Accuracy
-  ARGeoTrackingStatus.Accuracy.low 

Case

# ARGeoTrackingStatus.Accuracy.low

Geo-tracking accuracy is low.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case low
```

## Discussion

This value indicates that visual localization is complete and geo-tracking accuracy is low.

One technique an app can use to deal with low accuracy is to render location anchors with an asset that’s more forgiving, like a large ball. If an app renders the ball further in the air, any offset that results from low accuracy will be less noticeable, and less critical to the user.

## See Also

### Accuracies

case high

Geo-tracking accuracy is high.

case undetermined

Geo-tracking accuracy is undetermined.

case medium

Geo-tracking accuracy is average.

