

- BrowserEngineCore
-  BE_KEVENT_RETURN_IMMEDIATELY 

Global Variable

# BE_KEVENT_RETURN_IMMEDIATELY

Indicates that a request to receive kernel events needs to return without waiting for events.

iOS 17.4+iPadOS 17.4+

``` source
var BE_KEVENT_RETURN_IMMEDIATELY: Int32 { get }
```

## Overview

Use this constant in the `be_flags` parameter of be_kevent(_:_:_:_:_:_:), or the `flags` parameter of be_kevent64(_:_:_:_:_:_:), to poll for kernel events.

## See Also

### Kernel events

func be_kevent(Int32, UnsafePointer&lt;kevent>!, Int32, UnsafeMutablePointer&lt;kevent>!, Int32, UInt32) -> Int32

Registers for kernel events on the specified queue, and returns events that are pending on the queue, using 32-bit data types.

func be_kevent64(Int32, UnsafePointer&lt;kevent64_s>!, Int32, UnsafeMutablePointer&lt;kevent64_s>!, Int32, UInt32) -> Int32

Registers for kernel events on the specified queue, and returns events that are pending on the queue, using 64-bit data types.

var BE_KEVENT_NO_FLAGS: Int32

Indicates that no flags are set in a request to receive kernel events.

