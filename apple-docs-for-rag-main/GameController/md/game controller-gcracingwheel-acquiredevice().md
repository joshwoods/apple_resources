

- Game Controller
- GCRacingWheel
-  acquireDevice() 

Instance Method

# acquireDevice()

Starts receiving events from the racing wheel.

Mac Catalyst 16.0+macOS 13.0+

``` source
func acquireDevice() throws
```

## Discussion

Before invoking this method, the racing wheel doesn’t deliver events to your app. Since only one app may receive racing wheel events at a time, this method can fail to acquire the device.

## See Also

### Getting events

func relinquishDevice()

Stops receiving events from the racing wheel.

var isAcquired: Bool

A Boolean value that indicates whether the racing wheel sends events to the app.

