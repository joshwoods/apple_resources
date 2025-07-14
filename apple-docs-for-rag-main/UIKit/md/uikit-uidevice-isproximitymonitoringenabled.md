

- UIKit
- UIDevice
-  isProximityMonitoringEnabled 

Instance Property

# isProximityMonitoringEnabled

A Boolean value that indicates whether proximity monitoring is enabled.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isProximityMonitoringEnabled: Bool { get set }
```

## Discussion

Enable proximity monitoring only when your application needs to be notified of changes to the proximity state. Otherwise, disable proximity monitoring. The default value is false.

Not all iOS devices have proximity sensors. To determine if proximity monitoring is available, attempt to enable it. If the value of the isProximityMonitoringEnabled property remains false, proximity monitoring isn’t available.

## See Also

### Using the proximity sensor

var proximityState: Bool

A Boolean value that indicates whether the proximity sensor is close to the user.

