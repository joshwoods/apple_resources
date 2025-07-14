

- Foundation
- ProcessInfo
- ProcessInfo.ThermalState
-  ProcessInfo.ThermalState.fair 

Case

# ProcessInfo.ThermalState.fair

The thermal state is slightly elevated.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.10.3+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
case fair
```

## Discussion

The system takes steps to reduce thermal state, like running fans and stopping background services that aren’t doing work immediately needed by the user.

Reduce or defer background work, like prefetching content over the network or updating database indexes.

## See Also

### Constants

case nominal

The thermal state is within normal limits.

case serious

The thermal state is high.

case critical

The thermal state is significantly impacting the performance of the system and the device needs to cool down.

case nominal

The thermal state is within normal limits.

case serious

The thermal state is high.

case critical

The thermal state is significantly impacting the performance of the system and the device needs to cool down.

