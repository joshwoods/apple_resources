

- IOKit
-  IODataQueueClient.h 

API Collection

# IODataQueueClient.h

## Overview

### Included Headers

- \

- \

- \

- \

- \

- \

## Topics

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

func IODataQueueWaitForAvailableData(UnsafeMutablePointer&lt;IODataQueueMemory>!, mach_port_t) -> IOReturn

Wait for an incoming dataAvailable message on the given notifyPort.

