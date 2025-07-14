

- Foundation
- ProcessInfo
-  activeProcessorCount 

Instance Property

# activeProcessorCount

The number of active processing cores available on the computer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var activeProcessorCount: Int { get }
```

## Discussion

Whereas the processorCount property reports the number of advertised processing cores, the activeProcessorCount property reflects the actual number of active processing cores on the system. There are a number of different factors that may cause a core to not be active, including boot arguments, thermal throttling, or a manufacturing defect.

This property value is equal to the result of entering the command `sysctl -n hw.logicalcpu` on the current system.

## See Also

### Getting Computer Information

var processorCount: Int

The number of processing cores available on the computer.

var physicalMemory: UInt64

The amount of physical memory on the computer in bytes.

func isDeviceCertified(for: NSDeviceCertification) -> Bool

Indicates whether the device supports the requested performance tier.

func hasPerformanceProfile(NSProcessPerformanceProfile) -> Bool

Indicates whether an app is running under a known performance profile.

var systemUptime: TimeInterval

The amount of time the system has been awake since the last time it was restarted.

