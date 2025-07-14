

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOGatedOutputQueue
-  output(IOMbufQueue \*, UInt32 \*) 

# output(IOMbufQueue \*, UInt32 \*)

Transfers all packets in the mbuf queue to the target.

``` source
virtual void output(
 IOMbufQueue *queue,
 UInt32 *state); 
```

## Parameters 

`queue`  

A queue of output packets.

`state`  

Return a state bit defined by IOBasicOutputQueue that declares the new state of the queue following this method call. A kStateStalled is returned if the queue should stall, otherwise 0 is returned.

## See Also

### Miscellaneous

free

Frees the IOGatedOutputQueue object.

init

Initializes an IOGatedOutputQueue object.

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

