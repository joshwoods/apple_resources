

- MetricKit
- MXMetricManager
-  add(\_:) 

Instance Method

# add(\_:)

Registers to receive a daily report of app metrics from the metrics manager.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 12.0+visionOS 1.0+

``` source
func add(_ subscriber: any MXMetricManagerSubscriber)
```

## Parameters 

`subscriber`  

The object that receives the daily metrics reports. The object must conform to MXMetricManagerSubscriber.

## Discussion

Warning

If you call this function from a method that deallocates the object, your app might crash.

## See Also

### Subscribing to reports

func remove(any MXMetricManagerSubscriber)

Unsubscribes from daily reports of app metrics.

