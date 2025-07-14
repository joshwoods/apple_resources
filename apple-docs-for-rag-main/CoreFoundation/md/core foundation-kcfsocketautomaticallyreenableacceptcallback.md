

- Core Foundation
-  kCFSocketAutomaticallyReenableAcceptCallBack 

Global Variable

# kCFSocketAutomaticallyReenableAcceptCallBack

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var kCFSocketAutomaticallyReenableAcceptCallBack: CFOptionFlags { get }
```

## Discussion

When enabled using CFSocketSetSocketFlags(_:_:), the accept callback is called every time someone connects to your socket. When disabled, the accept callback is called only once the next time a new socket connection is accepted. The accept callback is automatically reenabled by default.

## See Also

### Constants

var kCFSocketAutomaticallyReenableReadCallBack: CFOptionFlags

var kCFSocketAutomaticallyReenableDataCallBack: CFOptionFlags

var kCFSocketAutomaticallyReenableWriteCallBack: CFOptionFlags

var kCFSocketLeaveErrors: CFOptionFlags

var kCFSocketCloseOnInvalidate: CFOptionFlags

When enabled using CFSocketSetSocketFlags(_:_:), the native socket associated with a CFSocket object is closed when the CFSocket object is invalidated. When disabled, the native socket remains open. This option is enabled by default.

