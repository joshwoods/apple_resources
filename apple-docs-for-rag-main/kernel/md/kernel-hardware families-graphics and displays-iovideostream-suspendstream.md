

- Kernel
- Hardware Families
- Graphics and Displays
- IOVideoStream
-  suspendStream 

# suspendStream

Temporarily suspend data flow on the stream.

``` source
virtual IOReturn suspendStream(
 void); 
```

## Return Value

Returns kIOReturnSuccess if the stream was successfully suspended.

## See Also

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

withBuffers

