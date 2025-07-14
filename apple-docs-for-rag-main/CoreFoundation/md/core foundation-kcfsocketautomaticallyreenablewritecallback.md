

- Core Foundation
-  kCFSocketAutomaticallyReenableWriteCallBack 

Global Variable

# kCFSocketAutomaticallyReenableWriteCallBack

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var kCFSocketAutomaticallyReenableWriteCallBack: CFOptionFlags { get }
```

## Discussion

When enabled using CFSocketSetSocketFlags(_:_:), the write callback is called every time more data can be written to the socket. When disabled, the write callback is called only the next time data can be written. The write callback is not automatically reenabled by default.

## See Also

### Constants

var kCFSocketAutomaticallyReenableReadCallBack: CFOptionFlags

var kCFSocketAutomaticallyReenableAcceptCallBack: CFOptionFlags

var kCFSocketAutomaticallyReenableDataCallBack: CFOptionFlags

var kCFSocketLeaveErrors: CFOptionFlags

var kCFSocketCloseOnInvalidate: CFOptionFlags

When enabled using CFSocketSetSocketFlags(_:_:), the native socket associated with a CFSocket object is closed when the CFSocket object is invalidated. When disabled, the native socket remains open. This option is enabled by default.

