

- IOKit
- IODataQueueClient.h
-  IODataQueuePeek(\_:) 

Function

# IODataQueuePeek(\_:)

Used to peek at the next entry on the queue.

iOS 18.4+iPadOS 18.4+Mac Catalyst 13.0+macOS 10.0+visionOS 2.4+

``` source
func IODataQueuePeek(_ dataQueue: UnsafeMutablePointer!) -> UnsafeMutablePointer!
```

## Parameters 

`dataQueue`  

The IODataQueueMemory region mapped from the kernel.

## Return Value

Returns a pointer to the next IODataQueueEntry if one is available. Zero is returned if the queue is empty.

## Discussion

This function can be used to look at the next entry which allows the entry to be received without having to copy it with IODataQueueDequeue. In order to do this, call IODataQueuePeek to get the entry. Then call IODataQueueDequeue with a NULL data pointer. That will cause the head to be moved to the next entry, but no memory to be copied.

## See Also

### Miscellaneous

func IODataQueueAllocateNotificationPort() -> mach_port_t

Allocates and returns a new mach port able to receive data available notifications from an IODataQueue.

func IODataQueueDataAvailable(UnsafeMutablePointer&lt;IODataQueueMemory>!) -> Bool

Used to determine if more data is avilable on the queue.

func IODataQueueDequeue(UnsafeMutablePointer&lt;IODataQueueMemory>!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;UInt32>!) -> IOReturn

Dequeues the next available entry on the queue and copies it into the given data pointer.

func IODataQueueEnqueue(UnsafeMutablePointer&lt;IODataQueueMemory>!, UnsafeMutableRawPointer!, UInt32) -> IOReturn

Enqueues a new entry on the queue.

func IODataQueueSetNotificationPort(UnsafeMutablePointer&lt;IODataQueueMemory>!, mach_port_t) -> IOReturn

Creates a simple mach message targeting the mach port specified in port.

func IODataQueueWaitForAvailableData(UnsafeMutablePointer&lt;IODataQueueMemory>!, mach_port_t) -> IOReturn

Wait for an incoming dataAvailable message on the given notifyPort.

