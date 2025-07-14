

- App Store Connect API
-  diagnosticLogs 

Object

# diagnosticLogs

A response containing log data for a diagnostic signature.

App Store Connect API 2.0+

``` source
object diagnosticLogs
```

## Properties

`productData`

`[`diagnosticLogs.ProductData`]`

An array of log data for a specific diagnostic signature.

`version`

`string`

The version of the App Store Connect API.

## Topics

### Objects

object diagnosticLogs.ProductData

The logs and insights for a diagnostic signature.

## See Also

### Objects and Types

object xcodeMetrics

A response that contains power and performance measurements for your app.

object DiagnosticInsight

The data structure that represents the Diagnostic Insight resource.

object DiagnosticSignaturesResponse

A response that contains a list of Diagnostic Signature resources.

object DiagnosticSignature

The data structure that represents the Diagnostic Signatures resource.

object DiagnosticLog

The data structure that represents the Diagnostic Logs resource.

object DiagnosticLogCallStackNode

Diagnostic information that describes a single line in a call stack.

object MetricsInsight

Results of an analysis of metric data for a single metric category for your app.

type MetricCategory

Categories of metric reports for apps that you distribute through the App Store.

object PerfPowerMetric

Unused.

