

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOGatedOutputQueue
-  scheduleServiceThread 

# scheduleServiceThread

Overrides the method inherited from IOOutputQueue.

``` source
virtual bool scheduleServiceThread(
 void *param); 
```

## Return Value

Returns true if a thread was successfully scheduled to service the queue.

## See Also

### Miscellaneous

free

Frees the IOGatedOutputQueue object.

init

Initializes an IOGatedOutputQueue object.

output(IOMbufQueue *, UInt32 *)

Transfers all packets in the mbuf queue to the target.

output(void *)

Overrides the method inherited from IOOutputQueue.

withTarget(IONetworkController *, IOWorkLoop *, UInt32)

Factory method that constructs and initializes an IOGatedOutputQueue object.

withTarget(IONetworkController *, IOWorkLoop *, UInt32, UInt32)

Factory method that constructs and initializes an IOGatedOutputQueue object.

withTarget(OSObject *, IOOutputAction, IOWorkLoop *, UInt32)

Factory method that constructs and initializes an IOGatedOutputQueue object.

withTarget(OSObject *, IOOutputAction, IOWorkLoop *, UInt32, UInt32)

Factory method that constructs and initializes an IOGatedOutputQueue object.

