

- Foundation
- ProcessInfo
- ProcessInfo.ThermalState
-  ProcessInfo.ThermalState.critical 

Case

# ProcessInfo.ThermalState.critical

The thermal state is significantly impacting the performance of the system and the device needs to cool down.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.10.3+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
case critical
```

## Discussion

The system takes significant steps to reduce thermal state. Fans are running at maximum speed.

Reduce usage of the CPU, GPU, and I/O such as Bluetooth or network to the minimum level required for user interaction. If possible, stop using peripherals such as the camera, flash, microphone, and speaker.

## See Also

### Constants

case nominal

The thermal state is within normal limits.

case fair

The thermal state is slightly elevated.

case serious

The thermal state is high.

case nominal

The thermal state is within normal limits.

case fair

The thermal state is slightly elevated.

case serious

The thermal state is high.

