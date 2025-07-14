

- SCSIPeripheralsDriverKit
- SCSIDeviceInParameters
-  fRealizedByteCountOfTransfer 

Instance Property

# fRealizedByteCountOfTransfer

The byte count of the tranferred data.

DriverKit 22.0+

``` source
uint64_t fRealizedByteCountOfTransfer;
```

## See Also

### Accessing response properties

fCompletionStatus

The status of the task at completion of the call, such as good, busy, or timeout.

fServiceResponse

The response from the service, such as complete, in process, or rejected.

fSenseDataValid

A Boolean value that indicates whether the sense data that the kernel provides is valid.

