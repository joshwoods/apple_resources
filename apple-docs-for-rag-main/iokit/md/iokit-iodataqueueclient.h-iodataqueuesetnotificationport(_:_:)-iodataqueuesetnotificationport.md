

- IOKit
- IODataQueueClient.h
-  IODataQueueSetNotificationPort(\_:\_:) 

Function

# IODataQueueSetNotificationPort(\_:\_:)

Creates a simple mach message targeting the mach port specified in port.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.5+visionOS 1.0+

``` source
func IODataQueueSetNotificationPort(
    _ dataQueue: UnsafeMutablePointer!,
    _ notifyPort: mach_port_t
) -> IOReturn
```

## Parameters 

`dataQueue`  

The IODataQueueMemory region mapped from the kernel created from an IOSharedDataQueue.

`notifyPort`  

The mach port to target with the notification message.

## Return Value

Returns kIOReturnSuccess on success. Returns kIOReturnBadArgument if either dataQueue is 0 (NULL).

## Discussion

This message is sent when data is added to an empty queue. It is to notify another user process that new data has become available. **Please note that using this method without mapped memory create from an IOSharedDataQueue will result in undefined behavior.**

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

func IODataQueuePeek(UnsafeMutablePointer&lt;IODataQueueMemory>!) -> UnsafeMutablePointer&lt;IODataQueueEntry>!

Used to peek at the next entry on the queue.

func IODataQueueWaitForAvailableData(UnsafeMutablePointer&lt;IODataQueueMemory>!, mach_port_t) -> IOReturn

Wait for an incoming dataAvailable message on the given notifyPort.

