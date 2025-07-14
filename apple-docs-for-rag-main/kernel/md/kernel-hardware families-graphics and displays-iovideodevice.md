

- Kernel
- Hardware Families
- Graphics and Displays
-  IOVideoDevice 

Class

# IOVideoDevice

A class that represents a video device.

macOS 10.7+

``` source
class IOVideoDevice : IOService
```

## Topics

### Miscellaneous

getStream

getStreamCount

newUserClient

See the documentation for the IOService method newUserClient.

setStreamMode

Sets the mode of the stream, either input or output.

startStream

Start sending data on a stream.

stopStream

Stop sending data on a stream.

suspendStream

Temporarily suspend data flow on the stream.

### Instance Methods

- addStream

- closeStream

- free

- getMetaClass

- getStream

- getStreamCount

- init

- inputCallback

- inputSyncCallback

- newUserClient

- openStream

- registerNotificationPort

- releaseStreams

- removeStream

- sendMultiNotification

- sendSingleNotification

- setControlValue

- setStreamFormat

- setStreamMode

- startStream

- startStream

- stopStream

- stopStream

- suspendStream

- suspendStream

## Relationships

### Inherits From

- IOService

## See Also

### Video

IONVRAMController

IOVideoControlDictionary

IOVideoStream

A class representing a stream of video data buffers passed from kernel to user space and back again.

IOVideoStreamDictionary

IOVideoStreamFormatDictionary

