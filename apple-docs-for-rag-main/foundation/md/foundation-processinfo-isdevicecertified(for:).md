

- Foundation
- ProcessInfo
-  isDeviceCertified(for:) 

Instance Method

# isDeviceCertified(for:)

Indicates whether the device supports the requested performance tier.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func isDeviceCertified(for performanceTier: NSDeviceCertification) -> Bool
```

## Parameters 

`performanceTier`  

The desired system performance tier. iPhonePerformanceGaming is the only performance tier.

## Return Value

`True` if the device meets the requirements for the given performance tier.

## See Also

### Getting Computer Information

var processorCount: Int

The number of processing cores available on the computer.

var activeProcessorCount: Int

The number of active processing cores available on the computer.

var physicalMemory: UInt64

The amount of physical memory on the computer in bytes.

func hasPerformanceProfile(NSProcessPerformanceProfile) -> Bool

Indicates whether an app is running under a known performance profile.

var systemUptime: TimeInterval

The amount of time the system has been awake since the last time it was restarted.

