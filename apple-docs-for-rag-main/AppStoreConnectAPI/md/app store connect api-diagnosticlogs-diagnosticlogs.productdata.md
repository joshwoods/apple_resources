

- App Store Connect API
- diagnosticLogs
-  diagnosticLogs.ProductData 

Object

# diagnosticLogs.ProductData

The logs and insights for a diagnostic signature.

App Store Connect API 2.0+

``` source
object diagnosticLogs.ProductData
```

## Properties

`signatureId`

`string`

The opaque resource ID that uniquely identifies a diagnostic signature.

`diagnosticInsights`

`[`diagnosticLogs.ProductData.DiagnosticInsights`]`

An array of insights for a diagnostic signature.

`diagnosticLogs`

`[`diagnosticLogs.ProductData.DiagnosticLogs`]`

An array of logs associated with a diagnostic signature.

## Topics

### Objects

object diagnosticLogs.ProductData.DiagnosticInsights

Information about an insight including a descriptive string, category, and URL.

object diagnosticLogs.ProductData.DiagnosticLogs

The call stack representation and metadata of the diagnostic log.

type DiagnosticInsightDirection

A string that describes the diagnostic insight direction.

type DiagnosticInsightType

A string that desribes the diagnostic insight type.

