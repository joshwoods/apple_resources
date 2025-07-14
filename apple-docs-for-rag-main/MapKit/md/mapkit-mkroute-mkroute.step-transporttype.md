

- MapKit
- MKRoute
- MKRoute.Step
-  transportType 

Instance Property

# transportType

The transport type of the step.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var transportType: MKDirectionsTransportType { get }
```

## Discussion

This property reflects the transport type employed by the step and may differ from the transport type of the overall route.

## See Also

### Getting additional step details

var instructions: String

The written instructions for following the path that the step represents.

var notice: String?

Additional notices that apply to the step.

var distance: CLLocationDistance

The step distance, in meters.

