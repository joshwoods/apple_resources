

- MapKit
- MKRoute
-  steps 

Instance Property

# steps

The array of steps that create the overall route.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var steps: [MKRoute.Step] { get }
```

## Discussion

The array contains one or more MKRoute.Step objects representing distinct portions of the route. Each step corresponds to a single direction that must be followed along the route.

## See Also

### Getting the route geometry

var polyline: MKPolyline

The detailed route geometry.

class Step

One portion of an overall route.

