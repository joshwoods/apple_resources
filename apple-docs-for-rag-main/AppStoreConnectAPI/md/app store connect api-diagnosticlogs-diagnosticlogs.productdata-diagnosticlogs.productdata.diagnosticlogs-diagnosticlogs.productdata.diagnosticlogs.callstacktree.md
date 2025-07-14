

- App Store Connect API
- diagnosticLogs
- diagnosticLogs.ProductData
- diagnosticLogs.ProductData.DiagnosticLogs
-  diagnosticLogs.ProductData.DiagnosticLogs.CallStackTree 

Object

# diagnosticLogs.ProductData.DiagnosticLogs.CallStackTree

The call stack representation of the diagnostic logs for single or multiple threads.

App Store Connect API 2.0+

``` source
object diagnosticLogs.ProductData.DiagnosticLogs.CallStackTree
```

## Properties

`callStackPerThread`

`boolean`

A Boolean value that indicates whether the call stack representation supports multiple threads.

`callStacks`

`[`diagnosticLogs.ProductData.DiagnosticLogs.CallStackTree.CallStacks`]`

The call stack representation of the diagnostic log.

## Topics

### Objects

object diagnosticLogs.ProductData.DiagnosticLogs.CallStackTree.CallStacks

The root call stack frames of the diagnostic log.

## See Also

### Objects

object diagnosticLogs.ProductData.DiagnosticLogs.DiagnosticMetaData

Information about the diagnostic log including app version and build information, event details, OS, device type, and platform, and disk writes.

