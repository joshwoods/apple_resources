

- MetricKit
- MXMetricManagerSubscriber
-  didReceive(\_:) 

Instance Method

# didReceive(\_:)

Delivers new diagnostic reports to the object registered with the metrics manager.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 12.0+visionOS 1.0+

``` source
optional func didReceive(_ payloads: [MXDiagnosticPayload])
```

## Parameters 

`payloads`  

An array of new diagnostic reports.

## Discussion

The system calls this method at most once per day. It’s safe to process the payload on a separate thread.

## See Also

### Receiving reports

func didReceive([MXMetricPayload])

Delivers new metrics reports to the object registered with the metrics manager.

