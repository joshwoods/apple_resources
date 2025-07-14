

- MapKit
- MKRoute
- MKRoute.Step
-  distance 

Instance Property

# distance

The step distance, in meters.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var distance: CLLocationDistance { get }
```

## Discussion

This property reflects the distance that the user covers while traversing the path of the step. It isn’t a lilnear distance between the start and end points of the step.

## See Also

### Getting additional step details

var instructions: String

The written instructions for following the path that the step represents.

var notice: String?

Additional notices that apply to the step.

var transportType: MKDirectionsTransportType

The transport type of the step.

