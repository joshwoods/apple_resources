

- MetricKit
- MXMetaData
-  applicationBuildVersion 

Instance Property

# applicationBuildVersion

The value of the bundle version key in the app’s property list.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 12.0+visionOS 1.0+

``` source
var applicationBuildVersion: String { get }
```

## Discussion

Returns the value of CFBundleVersion from this app’s information property list.

## See Also

### Reading data about a payload

var deviceType: String

The hardware identifier for the device.

var isTestFlightApp: Bool

Indicates whether the app is registered with TestFlight.

var lowPowerModeEnabled: Bool

Indicates whether low power mode is enabled on the device.

var osVersion: String

The version of the OS on the device including the type of OS, version number, and build number.

var platformArchitecture: String

The name of the processor architecture for the device.

var regionFormat: String

The short country code for the region format setting of the device.

var pid: pid_t

The process ID (PID) of the process.

