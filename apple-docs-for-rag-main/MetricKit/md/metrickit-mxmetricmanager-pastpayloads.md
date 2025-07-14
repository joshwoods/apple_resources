

- MetricKit
- MXMetricManager
-  pastPayloads 

Instance Property

# pastPayloads

Returns an array of the daily metrics reports generated since the last allocation of the shared manager instance.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var pastPayloads: [MXMetricPayload] { get }
```

## See Also

### Retrieving previous reports

var pastDiagnosticPayloads: [MXDiagnosticPayload]

Returns an array of the diagnostic reports generated since the last allocation of the shared manager instance.

