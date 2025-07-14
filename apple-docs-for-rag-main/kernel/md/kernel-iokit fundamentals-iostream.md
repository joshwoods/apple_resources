

- Kernel
- IOKit Fundamentals
-  IOStream 

Class

# IOStream

A class representing a stream of data buffers passed from kernel to user space and back again.

macOS 10.5+

``` source
class IOStream : IOService
```

## Overview

The IOStream class defines a mechanism for moving buffers of data from kernel space to user space or vice-versa. The policy for which direction the data flows and the nature of the data is left up the the implementer of the driver which uses IOStream.

Although it is expected that the client of an IOStream will be in user space, this is not required.

References to "output" mean "from the IOStream to the user client", and "input" means "from the user client to the IOStream."

## Topics

### Stream control

getStreamMode

Returns the mode of the stream, either input or output.

setStreamMode

Sets the mode of the stream, either input or output.

startStream

Start sending data on a stream.

stopStream

Stop sending data on a stream.

suspendStream

Temporarily suspend data flow on the stream.

### Queueing and dequeueing buffers

dequeueInputEntry

enqueueOutputBuffer

A convenience method for enqueueing a buffer.

enqueueOutputEntry

### Opening and closing streams

handleClose

The handleClose method destroys the shared input and output queues.

handleOpen

The handleOpen() method relies on the default IOService behavior to ensure that only one client has the stream open at a time. The shared input and output queues are created at open time.

### Managing user clients

newUserClient

See the documentation for the IOService method newUserClient.

### Managing shared queues

createQueues

Creates the shared input and output queues, without regard to whether the stream is open or not. Normally this is called by handleOpen().

destroyQueues

Releases the shared input and output queues.

getInputQueue

getInputQueueMemoryDescriptor

getOutputQueue

getOutputQueueMemoryDescriptor

### Managing notifications

inputCallback

Input callback function to be implemented by a subclass;

inputSyncCallback

Input callback function to be implemented by a subclass.

### Managing notification ports

getInputPort

Get the Mach port used to receive notifications from user space that a buffer has been added to the input queue.

getOutputPort

Get the Mach port used to send notifications to user space that a buffer has been added to the output queue.

sendOutputNotification

Send a notification to the user client that data is available for reading on the output queue. This will result in the user's output handler being called, if they registered one.

setInputPort

Set the Mach port used to receive notifications from user space that a buffer has been added to the input queue.

setOutputPort

Set the Mach port used to send notifications to user space that a buffer has been added to the output queue.

### Managing buffers in an IOStream

addBuffer

Add a buffer to an IOStream.

addBuffers

getBufferCount

getBuffers

Get an array containing all the buffers in the stream.

getBufferWithID

removeAllBuffers()

removeAllBuffers()

removeBuffer(IOStreamBuffer *)

Removes a buffer from the stream. Buffers cannot be removed while the stream is open, as this will change the buffer IDs of existing buffers.

removeBuffer(IOStreamBufferID)

Removes a buffer from the stream. Buffers cannot be removed while the stream is open, as this will change the buffer IDs of existing buffers.

### Creating IOStream objects

free

initWithBuffers

withBuffers

### Instance Methods

- addBuffer

- addBuffers

- createQueues

- dequeueInputEntry

- destroyQueues

- enqueueOutputBuffer

- enqueueOutputEntry

- free

- getBufferCount

- getBufferWithID

- getBuffers

- getInputPort

- getInputQueue

- getInputQueueMemoryDescriptor

- getMetaClass

- getOutputPort

- getOutputQueue

- getOutputQueueMemoryDescriptor

- getStreamMode

- handleClose

- handleOpen

- init

- initWithBuffers

- inputCallback

- inputSyncCallback

- newUserClient

- removeAllBuffers

- removeBuffer

- removeBuffer

- sendOutputNotification

- setInputPort

- setOutputPort

- setStreamMode

- startStream

- stopStream

- suspendStream

### Type Methods

+ withBuffers

## Relationships

### Inherits From

- IOService

## See Also

### User-Space Interactions

IOSharedDataQueue

A generic queue designed to pass data both from the kernel to a user process and from a user process to the kernel.

IOSharedInterruptController

IOUserClient

Provides a basis for communication between client applications and I/O Kit objects.

IOStreamUserClient

IOStreamBuffer

A class representing a data buffer that is part of an IOStream.

OSAction_IOUserClient_KernelCompletion

OSAction_IOUserClient_KernelCompletionInterface

