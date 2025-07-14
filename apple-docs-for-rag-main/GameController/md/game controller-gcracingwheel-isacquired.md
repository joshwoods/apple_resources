

- Game Controller
- GCRacingWheel
-  isAcquired 

Instance Property

# isAcquired

A Boolean value that indicates whether the racing wheel sends events to the app.

Mac Catalyst 16.0+macOS 13.0+

``` source
var isAcquired: Bool { get }
```

## See Also

### Getting events

func acquireDevice() throws

Starts receiving events from the racing wheel.

func relinquishDevice()

Stops receiving events from the racing wheel.

