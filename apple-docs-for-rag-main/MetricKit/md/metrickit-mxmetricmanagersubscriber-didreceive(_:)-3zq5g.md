

- MetricKit
- MXMetricManagerSubscriber
-  didReceive(\_:) 

Instance Method

# didReceive(\_:)

Delivers new metrics reports to the object registered with the metrics manager.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func didReceive(_ payloads: [MXMetricPayload])
```

## Parameters 

`payloads`  

An array of new metrics reports.

## Discussion

The system calls this method at most once per day. It’s safe to process the payload on a separate thread.

## See Also

### Receiving reports

func didReceive([MXDiagnosticPayload])

Delivers new diagnostic reports to the object registered with the metrics manager.

