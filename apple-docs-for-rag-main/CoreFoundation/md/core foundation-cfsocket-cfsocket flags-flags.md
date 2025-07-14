

- Core Foundation
- CFSocket
-  CFSocket Flags 

API Collection

# CFSocket Flags

Flags that can be set on a CFSocket object to control its behavior.

## Overview

The flags for a CFSocket object are set with CFSocketSetSocketFlags(_:_:). To immediately enable or disable a callback, use CFSocketEnableCallBacks(_:_:) and CFSocketDisableCallBacks(_:_:).

## Topics

### Constants

var kCFSocketAutomaticallyReenableReadCallBack: CFOptionFlags

var kCFSocketAutomaticallyReenableAcceptCallBack: CFOptionFlags

var kCFSocketAutomaticallyReenableDataCallBack: CFOptionFlags

var kCFSocketAutomaticallyReenableWriteCallBack: CFOptionFlags

var kCFSocketLeaveErrors: CFOptionFlags

var kCFSocketCloseOnInvalidate: CFOptionFlags

When enabled using CFSocketSetSocketFlags(_:_:), the native socket associated with a CFSocket object is closed when the CFSocket object is invalidated. When disabled, the native socket remains open. This option is enabled by default.

## See Also

### Constants

struct CFSocketCallBackType

Types of socket activity that can cause the callback function of a CFSocket object to be called.

enum CFSocketError

Error codes for many CFSocket functions.

