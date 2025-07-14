

- Foundation
- ProcessInfo
- ProcessInfo.ThermalState
-  ProcessInfo.ThermalState.serious 

Case

# ProcessInfo.ThermalState.serious

The thermal state is high.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.10.3+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
case serious
```

## Discussion

The system takes moderate steps to reduce thermal state, which reduces performance. Fans are running at maximum speed.

Reduce usage of resources that generate heat and consume battery, for example:

- Reduce or defer I/O operations, such as networking and Bluetooth

- Reduce the requested level of accuracy for location

- Reduce CPU and GPU usage by stopping or deferring work

- Reduce the target framerate from 60 FPS to 30 FPS

- Reduce the level of detail in rendered content by using fewer particles or lower-resolution textures

For more details on how to reduce your app’s use of these resources, see Energy Efficiency Guide for iOS Apps and Energy Efficiency Guide for Mac Apps.

## See Also

### Constants

case nominal

The thermal state is within normal limits.

case fair

The thermal state is slightly elevated.

case critical

The thermal state is significantly impacting the performance of the system and the device needs to cool down.

case nominal

The thermal state is within normal limits.

case fair

The thermal state is slightly elevated.

case critical

The thermal state is significantly impacting the performance of the system and the device needs to cool down.

