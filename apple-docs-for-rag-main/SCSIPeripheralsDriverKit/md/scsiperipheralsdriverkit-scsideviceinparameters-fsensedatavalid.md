

- SCSIPeripheralsDriverKit
- SCSIDeviceInParameters
-  fSenseDataValid 

Instance Property

# fSenseDataValid

A Boolean value that indicates whether the sense data that the kernel provides is valid.

DriverKit 22.0+

``` source
bool fSenseDataValid;
```

## Discussion

The default value of this property is `false`.

## See Also

### Accessing response properties

fCompletionStatus

The status of the task at completion of the call, such as good, busy, or timeout.

fServiceResponse

The response from the service, such as complete, in process, or rejected.

fRealizedByteCountOfTransfer

The byte count of the tranferred data.

