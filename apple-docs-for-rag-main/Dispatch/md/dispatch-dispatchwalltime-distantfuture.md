

- Dispatch
- DispatchWallTime
-  distantFuture 

Type Property

# distantFuture

A time in the distant future.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let distantFuture: DispatchWallTime
```

## Discussion

You can pass this value to methods that schedule work to have the system wait indefinitely for a particular event to occur or condition to be met.

## See Also

### Getting Well-Known Times

static func now() -> DispatchWallTime

Returns the current time.

