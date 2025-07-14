

- App Store Connect API
-  xcodeMetrics 

Object

# xcodeMetrics

A response that contains power and performance measurements for your app.

App Store Connect API 1.8+

``` source
object xcodeMetrics
```

## Properties

`insights`

xcodeMetrics.Insights

Analysis of data collected about the power and performance of your app that includes regressions and trends.

`productData`

`[`xcodeMetrics.ProductData`]`

An array of metrics data containing power and performance measurements for your app, organized by platform.

`version`

`string`

The current App Store Connect API version.

## Mentioned in 

App Store Connect API 2.0 release notes

## Topics

### Objects

object xcodeMetrics.Insights

Analysis of power and performance data collected for your app that includes regressions and trends.

object xcodeMetrics.ProductData

The metrics information of an app on a specific platform.

## See Also

### Objects and Types

object DiagnosticInsight

The data structure that represents the Diagnostic Insight resource.

object DiagnosticSignaturesResponse

A response that contains a list of Diagnostic Signature resources.

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

