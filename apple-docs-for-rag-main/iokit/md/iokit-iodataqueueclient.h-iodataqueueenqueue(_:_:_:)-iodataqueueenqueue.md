

- IOKit
- IODataQueueClient.h
-  IODataQueueEnqueue(\_:\_:\_:) 

Function

# IODataQueueEnqueue(\_:\_:\_:)

Enqueues a new entry on the queue.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.5+visionOS 1.0+

``` source
func IODataQueueEnqueue(
    _ dataQueue: UnsafeMutablePointer!,
    _ data: UnsafeMutableRawPointer!,
    _ dataSize: UInt32
) -> IOReturn
```

## Parameters 

`dataQueue`  

The IODataQueueMemory region mapped from the kernel created from an IOSharedDataQueue.

`data`  

Pointer to the data to be added to the queue.

`dataSize`  

Size of the data pointed to by data.

## Return Value

Returns kIOReturnSuccess on success. Other return values possible are: kIOReturnOverrun - queue is full.

## Discussion

This method adds a new data entry of dataSize to the queue. It sets the size parameter of the entry pointed to by the tail value and copies the memory pointed to by the data parameter in place in the queue. Once that is done, it moves the tail to the next available location. When attempting to add a new entry towards the end of the queue and there isn't enough space at the end, it wraps back to the beginning.

If the queue is empty when a new entry is added, the port specified in IODataQueueSetNotificationPort will be used to send a message to the client process that data is now available.

**Please note that using this method without mapped memory create from an IOSharedDataQueue will result in undefined behavior.**

## See Also

### Miscellaneous

func IODataQueueAllocateNotificationPort() -> mach_port_t

Allocates and returns a new mach port able to receive data available notifications from an IODataQueue.

func IODataQueueDataAvailable(UnsafeMutablePointer&lt;IODataQueueMemory>!) -> Bool

Used to determine if more data is avilable on the queue.

func IODataQueueDequeue(UnsafeMutablePointer&lt;IODataQueueMemory>!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;UInt32>!) -> IOReturn

Dequeues the next available entry on the queue and copies it into the given data pointer.

func IODataQueuePeek(UnsafeMutablePointer&lt;IODataQueueMemory>!) -> UnsafeMutablePointer&lt;IODataQueueEntry>!

Used to peek at the next entry on the queue.

func IODataQueueSetNotificationPort(UnsafeMutablePointer&lt;IODataQueueMemory>!, mach_port_t) -> IOReturn

Creates a simple mach message targeting the mach port specified in port.

func IODataQueueWaitForAvailableData(UnsafeMutablePointer&lt;IODataQueueMemory>!, mach_port_t) -> IOReturn

Wait for an incoming dataAvailable message on the given notifyPort.

