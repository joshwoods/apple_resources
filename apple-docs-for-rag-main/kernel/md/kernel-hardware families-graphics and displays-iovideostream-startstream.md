

- Kernel
- Hardware Families
- Graphics and Displays
- IOVideoStream
-  startStream 

# startStream

Start sending data on a stream.

``` source
virtual IOReturn startStream(
 void); 
```

## Return Value

Returns kIOReturnSuccess if the stream was successfully started.

## See Also

### Miscellaneous

getStreamMode

Returns the mode of the stream, either input or output.

initWithBuffers

setStreamMode

Sets the mode of the stream, either input or output.

stopStream

Stop sending data on a stream.

suspendStream

Temporarily suspend data flow on the stream.

withBuffers

