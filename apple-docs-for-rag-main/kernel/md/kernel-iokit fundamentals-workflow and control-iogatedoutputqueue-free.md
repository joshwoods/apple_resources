

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOGatedOutputQueue
-  free 

# free

Frees the IOGatedOutputQueue object.

``` source
virtual void free(); 
```

## Overview

Release allocated resources, then call super::free().

## See Also

### Miscellaneous

init

Initializes an IOGatedOutputQueue object.

output(IOMbufQueue *, UInt32 *)

Transfers all packets in the mbuf queue to the target.

output(void *)

Overrides the method inherited from IOOutputQueue.

scheduleServiceThread

Overrides the method inherited from IOOutputQueue.

withTarget(IONetworkController *, IOWorkLoop *, UInt32)

Factory method that constructs and initializes an IOGatedOutputQueue object.

withTarget(IONetworkController *, IOWorkLoop *, UInt32, UInt32)

Factory method that constructs and initializes an IOGatedOutputQueue object.

withTarget(OSObject *, IOOutputAction, IOWorkLoop *, UInt32)

Factory method that constructs and initializes an IOGatedOutputQueue object.

withTarget(OSObject *, IOOutputAction, IOWorkLoop *, UInt32, UInt32)

Factory method that constructs and initializes an IOGatedOutputQueue object.

