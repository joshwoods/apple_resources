

- Core Foundation
-  kCFSocketLeaveErrors 

Global Variable

# kCFSocketLeaveErrors

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var kCFSocketLeaveErrors: CFOptionFlags { get }
```

## Discussion

Normally, the CFNetwork stack calls getsockopt(2) macOS Developer Tools Manual Page to read the error code from the socket prior to calling your write callback. This also has the effect of clearing any pending errors on the socket.

If this flag is set, this call is skipped so that you can check for specific socket errors in your write callback.

## See Also

### Constants

var kCFSocketAutomaticallyReenableReadCallBack: CFOptionFlags

var kCFSocketAutomaticallyReenableAcceptCallBack: CFOptionFlags

var kCFSocketAutomaticallyReenableDataCallBack: CFOptionFlags

var kCFSocketAutomaticallyReenableWriteCallBack: CFOptionFlags

var kCFSocketCloseOnInvalidate: CFOptionFlags

When enabled using CFSocketSetSocketFlags(_:_:), the native socket associated with a CFSocket object is closed when the CFSocket object is invalidated. When disabled, the native socket remains open. This option is enabled by default.

