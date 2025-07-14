

- ARKit
- ARGeoTrackingStatus
-  ARGeoTrackingStatus.Accuracy 

Enumeration

# ARGeoTrackingStatus.Accuracy

Values that are possible for the current accuracy of geo tracking.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
enum Accuracy
```

## Discussion

To ensure the best possible user experience, an app must monitor and react to the geo-tracking accuracy. When accuracy is ARGeoTrackingStatus.Accuracy.low, the app needs to show content that’s more forgiving if ARKit is off by a small distance. For example, if accuracy is ARGeoTrackingStatus.Accuracy.low, rendering a location anchor as a large ball several meters in the air is more appropriate than rendering an arrow that rests its point on a real-world surface. Because a larger ball isn’t meant to mark a precise location, any offset that results from low accuracy will be less noticeable to the user. Apps that need higher-precision location anchors need to wait for ARGeoTrackingStatus.Accuracy.medium or ARGeoTrackingStatus.Accuracy.high accuracy before revealing rendered location-anchors, or dismissing user instructions.

## Topics

### Accuracies

case high

Geo-tracking accuracy is high.

case undetermined

Geo-tracking accuracy is undetermined.

case low

Geo-tracking accuracy is low.

case medium

Geo-tracking accuracy is average.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Judging Accuracy

var accuracy: ARGeoTrackingStatus.Accuracy

The accuracy of geo tracking at the time the session captured the frame.

