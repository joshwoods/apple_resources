

- Foundation
- ProcessInfo
-  physicalMemory 

Instance Property

# physicalMemory

The amount of physical memory on the computer in bytes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var physicalMemory: UInt64 { get }
```

## See Also

### Getting Computer Information

var processorCount: Int

The number of processing cores available on the computer.

var activeProcessorCount: Int

The number of active processing cores available on the computer.

func isDeviceCertified(for: NSDeviceCertification) -> Bool

Indicates whether the device supports the requested performance tier.

func hasPerformanceProfile(NSProcessPerformanceProfile) -> Bool

Indicates whether an app is running under a known performance profile.

var systemUptime: TimeInterval

The amount of time the system has been awake since the last time it was restarted.

