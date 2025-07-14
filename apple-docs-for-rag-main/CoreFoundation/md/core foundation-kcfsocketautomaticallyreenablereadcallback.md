

- Core Foundation
-  kCFSocketAutomaticallyReenableReadCallBack 

Global Variable

# kCFSocketAutomaticallyReenableReadCallBack

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var kCFSocketAutomaticallyReenableReadCallBack: CFOptionFlags { get }
```

## Discussion

When enabled using CFSocketSetSocketFlags(_:_:), the read callback is called every time the sockets has data to be read. When disabled, the read callback is called only once the next time data are available. The read callback is automatically reenabled by default.

## See Also

### Constants

var kCFSocketAutomaticallyReenableAcceptCallBack: CFOptionFlags

var kCFSocketAutomaticallyReenableDataCallBack: CFOptionFlags

var kCFSocketAutomaticallyReenableWriteCallBack: CFOptionFlags

var kCFSocketLeaveErrors: CFOptionFlags

var kCFSocketCloseOnInvalidate: CFOptionFlags

When enabled using CFSocketSetSocketFlags(_:_:), the native socket associated with a CFSocket object is closed when the CFSocket object is invalidated. When disabled, the native socket remains open. This option is enabled by default.

