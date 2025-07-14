

- Foundation
- ProcessInfo
-  hasPerformanceProfile(\_:) 

Instance Method

# hasPerformanceProfile(\_:)

Indicates whether an app is running under a known performance profile.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func hasPerformanceProfile(_ performanceProfile: NSProcessPerformanceProfile) -> Bool
```

## Parameters 

`performanceProfile`  

The desired performance profile. Choose between: default and sustained.

## Return Value

True if the system is running under the given performance profile. If the profile isn’t sustained, the app might cause the device to throttle under a heavy workload.

## See Also

### Getting Computer Information

var processorCount: Int

The number of processing cores available on the computer.

var activeProcessorCount: Int

The number of active processing cores available on the computer.

var physicalMemory: UInt64

The amount of physical memory on the computer in bytes.

func isDeviceCertified(for: NSDeviceCertification) -> Bool

Indicates whether the device supports the requested performance tier.

var systemUptime: TimeInterval

The amount of time the system has been awake since the last time it was restarted.

