

- Kernel
- Hardware Families
- Graphics and Displays
- IOVideoDevice
-  newUserClient 

# newUserClient

See the documentation for the IOService method newUserClient.

``` source
virtual IOReturn newUserClient(
 task_t owningTask,
 void *securityID,
 UInt32 type,
 OSDictionary *properties,
 IOUserClient **handler); 
```

## See Also

### Miscellaneous

getStream

getStreamCount

setStreamMode

Sets the mode of the stream, either input or output.

startStream

Start sending data on a stream.

stopStream

Stop sending data on a stream.

suspendStream

Temporarily suspend data flow on the stream.

