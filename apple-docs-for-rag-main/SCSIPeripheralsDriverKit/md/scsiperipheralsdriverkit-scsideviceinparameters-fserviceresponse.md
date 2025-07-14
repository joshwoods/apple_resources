

- SCSIPeripheralsDriverKit
- SCSIDeviceInParameters
-  fServiceResponse 

Instance Property

# fServiceResponse

The response from the service, such as complete, in process, or rejected.

DriverKit 22.0+

``` source
SCSIServiceResponse fServiceResponse;
```

## Discussion

Use the values that SCSIServiceResponse defines to evaluate this field.

## See Also

### Accessing response properties

fCompletionStatus

The status of the task at completion of the call, such as good, busy, or timeout.

fRealizedByteCountOfTransfer

The byte count of the tranferred data.

fSenseDataValid

A Boolean value that indicates whether the sense data that the kernel provides is valid.

