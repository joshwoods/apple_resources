

- Kernel
- Hardware Families
- Graphics and Displays
-  IOVideoStream 

Class

# IOVideoStream

A class representing a stream of video data buffers passed from kernel to user space and back again.

macOS 10.7+

``` source
class IOVideoStream : IOStream
```

## Overview

The IOVideoStream class defines a mechanism for moving buffers of data from kernel space to user space or vice-versa. The policy for which direction the data flows and the nature of the data is left up the the implementer of the driver which uses IOStream.

Although it is expected that the client of an IOVideoStream will be in user space, this is not required.

References to "output" mean "from the IOVideoStream to the user client", and "input" means "from the user client to the IOVideoStream."

## Topics

### Miscellaneous

getStreamMode

Returns the mode of the stream, either input or output.

initWithBuffers

setStreamMode

Sets the mode of the stream, either input or output.

startStream

Start sending data on a stream.

stopStream

Stop sending data on a stream.

suspendStream

Temporarily suspend data flow on the stream.

withBuffers

### Instance Methods

- getDevice

- getMetaClass

- getStreamMode

- initWithBuffers

- setStreamMode

- startStream

- stopStream

- suspendStream

### Type Methods

+ withBuffers

## Relationships

### Inherits From

- IOStream

## See Also

### Video

IOVideoDevice

A class that represents a video device.

IONVRAMController

IOVideoControlDictionary

IOVideoStreamDictionary

IOVideoStreamFormatDictionary

