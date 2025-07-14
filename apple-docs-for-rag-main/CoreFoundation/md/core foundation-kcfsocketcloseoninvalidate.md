

- Core Foundation
-  kCFSocketCloseOnInvalidate 

Global Variable

# kCFSocketCloseOnInvalidate

When enabled using CFSocketSetSocketFlags(_:_:), the native socket associated with a CFSocket object is closed when the CFSocket object is invalidated. When disabled, the native socket remains open. This option is enabled by default.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var kCFSocketCloseOnInvalidate: CFOptionFlags { get }
```

## See Also

### Constants

var kCFSocketAutomaticallyReenableReadCallBack: CFOptionFlags

var kCFSocketAutomaticallyReenableAcceptCallBack: CFOptionFlags

var kCFSocketAutomaticallyReenableDataCallBack: CFOptionFlags

var kCFSocketAutomaticallyReenableWriteCallBack: CFOptionFlags

var kCFSocketLeaveErrors: CFOptionFlags

