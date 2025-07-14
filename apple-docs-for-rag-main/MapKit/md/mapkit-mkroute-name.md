

- MapKit
- MKRoute
-  name 

Instance Property

# name

The assigned name for the route.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var name: String { get }
```

## Discussion

The framework localizes the string in this property according to the user’s language preferences. You can display this string to the user from your app’s user interface so that the user can distinguish one route from another.

The string itself describes the route using one of the route’s significant features. For example, a route that uses a major highway for a significant portion of the route might use that highway for its name.

## See Also

### Getting additional route details

var hasHighways: Bool

A Boolean value that indicates whether the route contains highways.

var hasTolls: Bool

A Boolean value that indicates whether the route has tolls.

var advisoryNotices: [String]

An array of advisory notice strings for the route.

var distance: CLLocationDistance

The route distance, in meters.

var expectedTravelTime: TimeInterval

The expected travel time, in seconds.

var transportType: MKDirectionsTransportType

The overall route transport type.

