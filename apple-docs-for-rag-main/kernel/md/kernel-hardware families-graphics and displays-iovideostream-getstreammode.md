

- Kernel
- Hardware Families
- Graphics and Displays
- IOVideoStream
-  getStreamMode 

# getStreamMode

Returns the mode of the stream, either input or output.

``` source
virtual IOStreamMode getStreamMode(
 void); 
```

## Return Value

The mode of the stream, either kIOStreamModeInput (from user space to kernel space) or the default kIOStreamModeOutput (from kernel space to user space).

## See Also

### Miscellaneous

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

