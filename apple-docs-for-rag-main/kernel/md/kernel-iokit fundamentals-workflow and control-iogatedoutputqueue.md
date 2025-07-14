

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IOGatedOutputQueue 

Class

# IOGatedOutputQueue

An extension of an IOBasicOutputQueue.

macOS 10.0+

``` source
class IOGatedOutputQueue : IOBasicOutputQueue
```

## Overview

An IOCommandGate object is created by this queue and added to a work loop as an event source. All calls to the target by the consumer thread must occur with the gate closed. Therefore, all calls to the target of this type of queue will be serialized with any other thread that runs on the same work loop context. This is useful for network drivers that have a tight hardware coupling between the transmit and receive engines, and a single-threaded hardware access model is desirable.

## Topics

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

withTarget(IONetworkController *, IOWorkLoop *, UInt32, UInt32)

Factory method that constructs and initializes an IOGatedOutputQueue object.

withTarget(OSObject *, IOOutputAction, IOWorkLoop *, UInt32)

Factory method that constructs and initializes an IOGatedOutputQueue object.

withTarget(OSObject *, IOOutputAction, IOWorkLoop *, UInt32, UInt32)

Factory method that constructs and initializes an IOGatedOutputQueue object.

### Instance Methods

- free

- getMetaClass

- output

- scheduleServiceThread

### Type Methods

+ gatedOutput

+ restartDeferredOutput

+ withTarget

+ withTarget

## Relationships

### Inherits From

- IOBasicOutputQueue

## See Also

### Output Queues

IOBasicOutputQueue

A concrete implementation of an IOOutputQueue.

IOOutputQueue

A packet queue that supports multiple producers and a single consumer.

