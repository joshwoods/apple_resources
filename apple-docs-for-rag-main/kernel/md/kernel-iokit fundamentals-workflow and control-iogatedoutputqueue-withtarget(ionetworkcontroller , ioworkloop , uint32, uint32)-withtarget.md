

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOGatedOutputQueue
-  withTarget(IONetworkController \*, IOWorkLoop \*, UInt32, UInt32) 

# withTarget(IONetworkController \*, IOWorkLoop \*, UInt32, UInt32)

Factory method that constructs and initializes an IOGatedOutputQueue object.

``` source
static IOGatedOutputQueue * withTarget(
 IONetworkController *target, 
 IOWorkLoop *workloop, 
 UInt32capacity, 
 UInt32priorities); 
```

## Parameters 

`target`  

An IONetworkController object that will handle packets removed from the queue.

`workloop`  

A workloop object. An IOCommandGate object is created and added to this workloop as an event source.

`capacity`  

The initial capacity of the output queue.

`priorities`  

The number of traffic priorities supported

## Return Value

Returns an IOGatedOutputQueue object on success, or 0 otherwise.

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

scheduleServiceThread

Overrides the method inherited from IOOutputQueue.

withTarget(IONetworkController *, IOWorkLoop *, UInt32)

Factory method that constructs and initializes an IOGatedOutputQueue object.

withTarget(OSObject *, IOOutputAction, IOWorkLoop *, UInt32)

Factory method that constructs and initializes an IOGatedOutputQueue object.

withTarget(OSObject *, IOOutputAction, IOWorkLoop *, UInt32, UInt32)

Factory method that constructs and initializes an IOGatedOutputQueue object.

