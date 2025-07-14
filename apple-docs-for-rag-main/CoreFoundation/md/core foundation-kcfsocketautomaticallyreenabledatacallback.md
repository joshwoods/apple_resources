

- Core Foundation
-  kCFSocketAutomaticallyReenableDataCallBack 

Global Variable

# kCFSocketAutomaticallyReenableDataCallBack

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var kCFSocketAutomaticallyReenableDataCallBack: CFOptionFlags { get }
```

## Discussion

When enabled using CFSocketSetSocketFlags(_:_:), the data callback is called every time the socket has read some data. When disabled, the data callback is called only once the next time data are read. The data callback is automatically reenabled by default.

## See Also

### Constants

var kCFSocketAutomaticallyReenableReadCallBack: CFOptionFlags

var kCFSocketAutomaticallyReenableAcceptCallBack: CFOptionFlags

var kCFSocketAutomaticallyReenableWriteCallBack: CFOptionFlags

var kCFSocketLeaveErrors: CFOptionFlags

var kCFSocketCloseOnInvalidate: CFOptionFlags

When enabled using CFSocketSetSocketFlags(_:_:), the native socket associated with a CFSocket object is closed when the CFSocket object is invalidated. When disabled, the native socket remains open. This option is enabled by default.

