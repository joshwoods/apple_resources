

- MetricKit
- MXDiagnostic
-  applicationVersion 

Instance Property

# applicationVersion

The value of the bundle version key, short form, in the app’s property list.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 12.0+visionOS 1.0+

``` source
var applicationVersion: String { get }
```

## Discussion

Returns the value of CFBundleShortVersionString from this app’s information property list.

## See Also

### Reading data About a diagnostic

var metaData: MXMetaData

A set of system-level information for the device.

var signpostData: [MXSignpostRecord]?

