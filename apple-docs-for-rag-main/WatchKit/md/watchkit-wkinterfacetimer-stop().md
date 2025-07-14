

- WatchKit
- WKInterfaceTimer
-  stop() 

Instance Method

# stop()

Stops updates to the timer’s display.

watchOS 2.0+

``` source
func stop()
```

## Discussion

Use this method to stop updates to the timer object’s label. This method does not stop the timer from counting. The timer continues counting to or from its target value even when updates to the label are not occurring.

## See Also

### Starting and Stopping the Timer

func start()

Begins updates to the timer’s display.

