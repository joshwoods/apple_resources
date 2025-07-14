

- MapKit
- MKDirections
- MKDirections.Response
-  routes 

Instance Property

# routes

An array of route objects representing the directions between the start and end points.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var routes: [MKRoute] { get }
```

## Discussion

The array contains one or more MKRoute objects, each of which represents a possible set of directions for the user to follow. If you don’t request alternate routes in the original directions request, this array contains at most one object.

Each route object contains geometry information that you can use to display that route on your app’s map view. Routes may also contain additional information that’s relevant to that particular route, such as the expected travel time and any trip advisory notices.

