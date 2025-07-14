

- MapKit
- MKRoute
-  advisoryNotices 

Instance Property

# advisoryNotices

An array of advisory notice strings for the route.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var advisoryNotices: [String] { get }
```

## Discussion

This property contains an array of NSString objects. The framework localizes each string according to the user’s language preferences. The strings contain additional information that’s important for the user to know about the route. For example, a string might note the closing of a portion of the route during the winter or after big storms.

## See Also

### Getting additional route details

var name: String

The assigned name for the route.

var hasHighways: Bool

A Boolean value that indicates whether the route contains highways.

var hasTolls: Bool

A Boolean value that indicates whether the route has tolls.

var distance: CLLocationDistance

The route distance, in meters.

var expectedTravelTime: TimeInterval

The expected travel time, in seconds.

var transportType: MKDirectionsTransportType

The overall route transport type.

