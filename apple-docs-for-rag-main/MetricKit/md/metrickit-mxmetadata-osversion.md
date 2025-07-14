

- MetricKit
- MXMetaData
-  osVersion 

Instance Property

# osVersion

The version of the OS on the device including the type of OS, version number, and build number.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 12.0+visionOS 1.0+

``` source
var osVersion: String { get }
```

## Discussion

The OS version is the same as the one used in crash reports.

## See Also

### Reading data about a payload

var applicationBuildVersion: String

The value of the bundle version key in the app’s property list.

var deviceType: String

The hardware identifier for the device.

var isTestFlightApp: Bool

Indicates whether the app is registered with TestFlight.

var lowPowerModeEnabled: Bool

Indicates whether low power mode is enabled on the device.

var platformArchitecture: String

The name of the processor architecture for the device.

var regionFormat: String

The short country code for the region format setting of the device.

var pid: pid_t

The process ID (PID) of the process.

