

- MapKit
- MKRoute
- MKRoute.Step
-  instructions 

Instance Property

# instructions

The written instructions for following the path that the step represents.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var instructions: String { get }
```

## Discussion

The framework localizes the string in this property according to the user’s language preferences. You can present this string to the user from your app’s interface.

## See Also

### Getting additional step details

var notice: String?

Additional notices that apply to the step.

var distance: CLLocationDistance

The step distance, in meters.

var transportType: MKDirectionsTransportType

The transport type of the step.

