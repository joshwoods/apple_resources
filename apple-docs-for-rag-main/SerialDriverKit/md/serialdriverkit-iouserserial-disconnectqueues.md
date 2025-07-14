

- SerialDriverKit
- IOUserSerial
-  DisconnectQueues 

Instance Method

# DisconnectQueues

Releases the buffers that manage data moving to and from the device.

DriverKit 19.0+

``` source
kern_return_t DisconnectQueues();
```

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

During the cleanup of your driver, call this method to disconnect the data queues you use to buffer data. If you provided the buffer objects at configuration time, the system releases its references to the objects you provided.

## See Also

### Configuring the Serial Data Queues

ConnectQueues

Creates and configures the buffers that store the data moving to and from the device.

