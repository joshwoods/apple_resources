

- Kernel
- Hardware Families
- Graphics and Displays
- IOVideoDevice
-  getStream 

# getStream

``` source
virtual IOVideoStream* getStream(
 UInt32streamIndex); 
```

## Parameters 

`streamIndex`  

The index for which the underlying stream is desired.

## Return Value

Returns the number of streams of the device.

## See Also

### Miscellaneous

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

