

- IOKit
- IODataQueueClient.h
-  IODataQueueWaitForAvailableData(\_:\_:) 

Function

# IODataQueueWaitForAvailableData(\_:\_:)

Wait for an incoming dataAvailable message on the given notifyPort.

iOS 18.4+iPadOS 18.4+Mac Catalyst 13.0+macOS 10.0+visionOS 2.4+

``` source
func IODataQueueWaitForAvailableData(
    _ dataQueue: UnsafeMutablePointer!,
    _ notificationPort: mach_port_t
) -> IOReturn
```

## Parameters 

`dataQueue`  

The IODataQueueMemory region mapped from the kernel.

`notifyPort`  

Mach port on which to listen for incoming messages.

## Return Value

Returns kIOReturnSuccess on success. Returns kIOReturnBadArgument if either dataQueue is 0 (NULL) or notiryPort is MACH_PORT_NULL. Returns the result of the mach_msg() listen call on the given port.

## Discussion

This method will simply wait for an incoming message on the given notifyPort. Once it is received, the return from mach_msg() is returned.

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

func IODataQueueSetNotificationPort(UnsafeMutablePointer&lt;IODataQueueMemory>!, mach_port_t) -> IOReturn

Creates a simple mach message targeting the mach port specified in port.

