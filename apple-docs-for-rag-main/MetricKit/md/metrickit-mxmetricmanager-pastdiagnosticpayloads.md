

- MetricKit
- MXMetricManager
-  pastDiagnosticPayloads 

Instance Property

# pastDiagnosticPayloads

Returns an array of the diagnostic reports generated since the last allocation of the shared manager instance.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 12.0+visionOS 1.0+

``` source
var pastDiagnosticPayloads: [MXDiagnosticPayload] { get }
```

## See Also

### Retrieving previous reports

var pastPayloads: [MXMetricPayload]

Returns an array of the daily metrics reports generated since the last allocation of the shared manager instance.

