

- MapKit
- MKRoute
-  polyline 

Instance Property

# polyline

The detailed route geometry.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var polyline: MKPolyline { get }
```

## Discussion

The polyline object in this property reflects the complete path of the route, including all of its steps. You can use the polyline object as an overlay in a map view.

## See Also

### Getting the route geometry

var steps: [MKRoute.Step]

The array of steps that create the overall route.

class Step

One portion of an overall route.

