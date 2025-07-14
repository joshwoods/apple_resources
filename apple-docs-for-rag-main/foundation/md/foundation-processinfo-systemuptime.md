

- Foundation
- ProcessInfo
-  systemUptime 

Instance Property

# systemUptime

The amount of time the system has been awake since the last time it was restarted.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var systemUptime: TimeInterval { get }
```

## Discussion

Important

This API has the potential of being misused to access device signals to try to identify the device or user, also known as fingerprinting. Regardless of whether a user gives your app permission to track, fingerprinting is not allowed. When you use this API in your app or third-party SDK (an SDK not provided by Apple), declare your usage and the reason for using the API in your app or third-party SDK’s `PrivacyInfo.xcprivacy` file. For more information, including the list of valid reasons for using the API, see Describing use of required reason API.

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

func hasPerformanceProfile(NSProcessPerformanceProfile) -> Bool

Indicates whether an app is running under a known performance profile.

