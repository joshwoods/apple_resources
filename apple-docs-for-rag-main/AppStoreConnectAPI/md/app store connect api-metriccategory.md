

- App Store Connect API
-  MetricCategory 

Type

# MetricCategory

Categories of metric reports for apps that you distribute through the App Store.

App Store Connect API 2.0+

``` source
string MetricCategory
```

## Possible Values 

`HANG`  

`LAUNCH`  

`MEMORY`  

`DISK`  

`BATTERY`  

`TERMINATION`  

`ANIMATION`  

### Possible values

HANG  
The number of seconds per hour that the main thread of the app is unresponsive for more than 250ms, which is the maximum amount of time an app can respond to a typical user event before the user perceives it as slow.

LAUNCH  
The average launch time, which is the time between the user tapping on your app icon and the time that the system draws a screen other than the launch screen. The launch time is measured in milliseconds.

MEMORY  
The amount of memory the app uses, in megabytes.

DISK  
The amount of megabytes per day the app writes to long term storage.

BATTERY  
The amount of battery power the app uses over a 24 hour period when the device is disconnected from power.

TERMINATION  
The average amount of non-user-initiated app terminations, including background terminations, per day.

ANIMATION  
The duration of pauses that occur while scrolling an app.

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

object MetricsInsight

Results of an analysis of metric data for a single metric category for your app.

object PerfPowerMetric

Unused.

