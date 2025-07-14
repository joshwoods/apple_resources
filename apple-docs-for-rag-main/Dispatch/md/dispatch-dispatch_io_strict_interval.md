

- Dispatch
-  DISPATCH_IO_STRICT_INTERVAL 

Global Variable

# DISPATCH_IO_STRICT_INTERVAL

Enqueue handlers for a channel at strict intervals regardless of how much data has been read or written.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var DISPATCH_IO_STRICT_INTERVAL: Int32 { get }
```

## Discussion

Setting this flag can lead to the handler being called even if the amount of data does not exceed the channel’s low-water mark.

## See Also

### Interval Flags

static let strictInterval: DispatchIO.IntervalFlags

Enqueue handlers for a channel at strict intervals regardless of how much data has been read or written.

