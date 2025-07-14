

- Kernel
- Hardware Families
- Graphics and Displays
- IOVideoDevice
-  setStreamMode 

# setStreamMode

Sets the mode of the stream, either input or output.

``` source
virtual IOReturn setStreamMode(
 IOVideoStream *stream,
 IOStreamMode mode); 
```

## Overview

This must be implemented by a subclass.

## See Also

### Miscellaneous

getStream

getStreamCount

newUserClient

See the documentation for the IOService method newUserClient.

startStream

Start sending data on a stream.

stopStream

Stop sending data on a stream.

suspendStream

Temporarily suspend data flow on the stream.

