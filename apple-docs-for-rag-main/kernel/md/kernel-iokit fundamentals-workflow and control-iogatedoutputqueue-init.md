

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOGatedOutputQueue
-  init 

# init

Initializes an IOGatedOutputQueue object.

``` source
virtual bool init(
 OSObject *target, 
 IOOutputAction action, 
 IOWorkLoop *workloop, 
 UInt32 capacity = 0, 
 UInt32 priorities = 1); 
```

## Parameters 

`target`  

The object that will handle packets removed from the queue, and is usually a subclass of IONetworkController.

`action`  

The function that will handle packets removed from the queue.

`workloop`  

A workloop object. An IOCommandGate object is created and added to this workloop as an event source.

`capacity`  

The initial capacity of the output queue.

## Return Value

Returns true if initialized successfully, false otherwise.

## See Also

### Miscellaneous

free

Frees the IOGatedOutputQueue object.

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

