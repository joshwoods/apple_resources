

- App Store Connect API
-  DiagnosticLogCallStackNode 

Object

# DiagnosticLogCallStackNode

Diagnostic information that describes a single line in a call stack.

App Store Connect API 2.0+

``` source
object DiagnosticLogCallStackNode
```

## Properties

`sampleCount`

`integer`

The number of samples that captured the frame. Samples are taken at consistent intervals, meaning a greater number of samples results in a greater value for the metric.

`isBlameFrame`

`boolean`

A Boolean value that indicates whether the frame is the responsibility of your app.

`binaryName`

`string`

The name of the binary responsible for the frame.

`binaryUUID`

`string`

The unique identifier of the binary image that contains the frame.

`symbolName`

`string`

The name of the symbol in your code.

`fileName`

`string`

The file name of the file where the frame is defined.

`address`

`string`

The memory address of the frame.

`insightsCategory`

`string`

The insight category that applies to the frame.

`lineNumber`

`string`

The line number where the function is invoked.

`offsetIntoBinaryTextSegment`

`string`

The number of bytes the frame is offset from the start of the binary text segment, for unsymbolicated frames.

`offsetIntoSymbol`

`string`

The number of bytes the frame is offset from the start of the function, for symbolicated frames.

`rawFrame`

`string`

The unparsed frame from the log.

`subFrames`

`[`DiagnosticLogCallStackNode`]`

An array of call stack frames.

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

object MetricsInsight

Results of an analysis of metric data for a single metric category for your app.

type MetricCategory

Categories of metric reports for apps that you distribute through the App Store.

object PerfPowerMetric

Unused.

