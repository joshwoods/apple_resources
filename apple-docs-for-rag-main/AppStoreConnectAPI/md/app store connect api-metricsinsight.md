

- App Store Connect API
-  MetricsInsight 

Object

# MetricsInsight

Results of an analysis of metric data for a single metric category for your app.

App Store Connect API 2.0+

``` source
object MetricsInsight
```

## Properties

`highImpact`

`boolean`

A Boolean value that indicates whether the insight is high impact, meaning the metrics show that the latest app version has a regression of 100% or more, compared with the average values of the metric from the previous app versions.

`metricCategory`

MetricCategory

The category of the metric that this insight is about.

`metric`

`string`

The specific measurement within the `metricCategory` that this insight analyzes.

`subSystemLabel`

`string`

A metric subtype, which provides additional information about the source of the measurement.

`latestVersion`

`string`

The version number of the most current version of the app.

`maxLatestVersionValue`

`number`

The maximum value of this metric for the latest app version, from the values in `populations`.

`populations`

`[`MetricsInsight.Populations`]`

An array of metrics organized by device type on the latest app version, that includes the percent change of the metric as compared with previous app versions.

`summaryString`

`string`

A human-readable description of the trend.

`referenceVersions`

`string`

A list of previous app versions that the system uses to compare the current app version to, when calculating metric value regressions or trends.

## Topics

### Objects

object MetricsInsight.Populations

The value of a metric for a device type on the latest app version, and its percent change as compared with previous app versions.

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

object diagnosticLogs

A response containing log data for a diagnostic signature.

object DiagnosticLog

The data structure that represents the Diagnostic Logs resource.

object DiagnosticLogCallStackNode

Diagnostic information that describes a single line in a call stack.

type MetricCategory

Categories of metric reports for apps that you distribute through the App Store.

object PerfPowerMetric

Unused.

