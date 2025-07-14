

- App Store Connect API
- diagnosticLogs
- diagnosticLogs.ProductData
-  diagnosticLogs.ProductData.DiagnosticLogs 

Object

# diagnosticLogs.ProductData.DiagnosticLogs

The call stack representation and metadata of the diagnostic log.

App Store Connect API 2.0+

``` source
object diagnosticLogs.ProductData.DiagnosticLogs
```

## Properties

`callStackTree`

`[`diagnosticLogs.ProductData.DiagnosticLogs.CallStackTree`]`

The call stack representation of the diagnostic log.

`diagnosticMetaData`

diagnosticLogs.ProductData.DiagnosticLogs.DiagnosticMetaData

Information about the diagnostic log the system captured.

## Topics

### Objects

object diagnosticLogs.ProductData.DiagnosticLogs.CallStackTree

The call stack representation of the diagnostic logs for single or multiple threads.

object diagnosticLogs.ProductData.DiagnosticLogs.DiagnosticMetaData

Information about the diagnostic log including app version and build information, event details, OS, device type, and platform, and disk writes.

## See Also

### Objects

object diagnosticLogs.ProductData.DiagnosticInsights

Information about an insight including a descriptive string, category, and URL.

type DiagnosticInsightDirection

A string that describes the diagnostic insight direction.

type DiagnosticInsightType

A string that desribes the diagnostic insight type.

