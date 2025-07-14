

- Dispatch
- DispatchIO
- DispatchIO.IntervalFlags
-  strictInterval 

Type Property

# strictInterval

Enqueue handlers for a channel at strict intervals regardless of how much data has been read or written.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let strictInterval: DispatchIO.IntervalFlags
```

## Discussion

Setting this flag can lead to the handler being called even if the amount of data does not exceed the channel’s low-water mark.

## See Also

### Interval Flags

var DISPATCH_IO_STRICT_INTERVAL: Int32

Enqueue handlers for a channel at strict intervals regardless of how much data has been read or written.

