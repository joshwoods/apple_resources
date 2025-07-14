

- App Store Connect API
-  DiagnosticSignaturesResponse 

Object

# DiagnosticSignaturesResponse

A response that contains a list of Diagnostic Signature resources.

App Store Connect API 1.2+

``` source
object DiagnosticSignaturesResponse
```

## Properties

`data`

`[`DiagnosticSignature`]`

 (Required) 

An array of diagnostic signatures.

`links`

PagedDocumentLinks

 (Required) 

Navigational links that include the self-link.

`meta`

PagingInformation

Paging information.

## See Also

### Objects and Types

object xcodeMetrics

A response that contains power and performance measurements for your app.

object DiagnosticInsight

The data structure that represents the Diagnostic Insight resource.

object DiagnosticSignature

The data structure that represents the Diagnostic Signatures resource.

object diagnosticLogs

A response containing log data for a diagnostic signature.

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

