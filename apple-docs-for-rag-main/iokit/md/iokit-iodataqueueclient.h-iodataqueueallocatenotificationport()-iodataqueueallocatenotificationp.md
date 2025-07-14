

- IOKit
- IODataQueueClient.h
-  IODataQueueAllocateNotificationPort() 

Function

# IODataQueueAllocateNotificationPort()

Allocates and returns a new mach port able to receive data available notifications from an IODataQueue.

iOS 18.4+iPadOS 18.4+Mac Catalyst 13.0+macOS 10.0+visionOS 2.4+

``` source
func IODataQueueAllocateNotificationPort() -> mach_port_t
```

## Return Value

Returns a newly allocated mach port on success. On failure, it returns MACH_PORT_NULL.

## Discussion

This port is intended to be passed down into the kernel and into an IODataQueue to allow it to send the appropriate notification. The returned mach port is allocated with a queue limit of one message. This allows only one mach message to be queued up at a time. The IODataQueue code is written with the restriction in mind and will only queue up a message if no messages alread have been sent.

## See Also

### Miscellaneous

func IODataQueueDataAvailable(UnsafeMutablePointer&lt;IODataQueueMemory>!) -> Bool

Used to determine if more data is avilable on the queue.

func IODataQueueDequeue(UnsafeMutablePointer&lt;IODataQueueMemory>!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;UInt32>!) -> IOReturn

Dequeues the next available entry on the queue and copies it into the given data pointer.

func IODataQueueEnqueue(UnsafeMutablePointer&lt;IODataQueueMemory>!, UnsafeMutableRawPointer!, UInt32) -> IOReturn

Enqueues a new entry on the queue.

func IODataQueuePeek(UnsafeMutablePointer&lt;IODataQueueMemory>!) -> UnsafeMutablePointer&lt;IODataQueueEntry>!

Used to peek at the next entry on the queue.

func IODataQueueSetNotificationPort(UnsafeMutablePointer&lt;IODataQueueMemory>!, mach_port_t) -> IOReturn

Creates a simple mach message targeting the mach port specified in port.

func IODataQueueWaitForAvailableData(UnsafeMutablePointer&lt;IODataQueueMemory>!, mach_port_t) -> IOReturn

Wait for an incoming dataAvailable message on the given notifyPort.

