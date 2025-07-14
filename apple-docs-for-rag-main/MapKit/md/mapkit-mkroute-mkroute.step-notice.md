

- MapKit
- MKRoute
- MKRoute.Step
-  notice 

Instance Property

# notice

Additional notices that apply to the step.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var notice: String? { get }
```

## Discussion

Notices may include legal information or warning notices that apply to the step. For example, if the step crosses railroad tracks, it might contain a notice that warns the user not to cross the tracks when the lights are flashing.

## See Also

### Getting additional step details

var instructions: String

The written instructions for following the path that the step represents.

var distance: CLLocationDistance

The step distance, in meters.

var transportType: MKDirectionsTransportType

The transport type of the step.

