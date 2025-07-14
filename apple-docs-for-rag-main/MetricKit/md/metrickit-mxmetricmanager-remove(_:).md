

- MetricKit
- MXMetricManager
-  remove(\_:) 

Instance Method

# remove(\_:)

Unsubscribes from daily reports of app metrics.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 12.0+visionOS 1.0+

``` source
func remove(_ subscriber: any MXMetricManagerSubscriber)
```

## Parameters 

`subscriber`  

The object that receives daily metrics reports. Passing an object that is not currently subscribed does nothing.

## Discussion

Warning

If you call this function from a method that deallocates the object, your app might crash.

## See Also

### Subscribing to reports

func add(any MXMetricManagerSubscriber)

Registers to receive a daily report of app metrics from the metrics manager.

