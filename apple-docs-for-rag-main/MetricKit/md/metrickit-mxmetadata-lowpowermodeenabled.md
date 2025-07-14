

- MetricKit
- MXMetaData
-  lowPowerModeEnabled 

Instance Property

# lowPowerModeEnabled

Indicates whether low power mode is enabled on the device.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var lowPowerModeEnabled: Bool { get }
```

## Discussion

Retrieve the current setting of the system for the low power mode setting. On systems where the low power mode is unknown or unsupported, the value returned from the lowPowerModeEnabled property is always NO.

## See Also

### Reading data about a payload

var applicationBuildVersion: String

The value of the bundle version key in the app’s property list.

var deviceType: String

The hardware identifier for the device.

var isTestFlightApp: Bool

Indicates whether the app is registered with TestFlight.

var osVersion: String

The version of the OS on the device including the type of OS, version number, and build number.

var platformArchitecture: String

The name of the processor architecture for the device.

var regionFormat: String

The short country code for the region format setting of the device.

var pid: pid_t

The process ID (PID) of the process.

