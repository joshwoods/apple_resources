

- Network Extension
- NEFilterNewFlowVerdict
-  statisticsReportFrequency 

Instance Property

# statisticsReportFrequency

The frequency at which the data provider receives reports.

macOS 10.15.4+

``` source
var statisticsReportFrequency: NEFilterReport.Frequency { get set }
```

## Discussion

This property determines the frequency at which the system calls the data provider’s handle(_:) method with an NEFilterReport instance that contains an NEFilterReport.Event.statistics event.

## See Also

### Inspecting new flow verdict properties

enum Frequency

An enumeration that represents the frequency of filter report delivery.

