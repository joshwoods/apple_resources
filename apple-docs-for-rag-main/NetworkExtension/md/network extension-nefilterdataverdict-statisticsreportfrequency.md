

- Network Extension
- NEFilterDataVerdict
-  statisticsReportFrequency 

Instance Property

# statisticsReportFrequency

The frequencty at which to provide flow statistics to the data provider.

macOS 10.15.4+

``` source
var statisticsReportFrequency: NEFilterReport.Frequency { get set }
```

## Discussion

This property determines the frequency at which the provider receives a call to its handle(_:) method with an NEFilterReport.Event.statistics event.

The default value of this property NEFilterReport.Frequency.none, meaning that the provider receives no statistics by default.

