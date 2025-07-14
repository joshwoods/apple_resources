

- App Store Connect API
-  DiagnosticSignature 

Object

# DiagnosticSignature

The data structure that represents the Diagnostic Signatures resource.

App Store Connect API 1.2+

``` source
object DiagnosticSignature
```

## Properties

`attributes`

DiagnosticSignature.Attributes

Attributes that describe the diagnostic signature resource.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies a diagnostic signature.

`links`

ResourceLinks

Navigational links that include the self-link.

`relationships`

DiagnosticSignature.Relationships

`type`

`string`

 (Required) 

The resource type.

Value: `diagnosticSignatures`

## Topics

### Objects

object DiagnosticSignature.Attributes

Attributes that describe a Diagnostic Signatures resource.

### Dictionaries

object DiagnosticSignature.Relationships

## See Also

### Objects and Types

object xcodeMetrics

A response that contains power and performance measurements for your app.

object DiagnosticInsight

The data structure that represents the Diagnostic Insight resource.

object DiagnosticSignaturesResponse

A response that contains a list of Diagnostic Signature resources.

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

