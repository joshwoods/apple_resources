

- SCSIPeripheralsDriverKit
- SCSIDeviceInParameters
-  fCompletionStatus 

Instance Property

# fCompletionStatus

The status of the task at completion of the call, such as good, busy, or timeout.

DriverKit 22.0+

``` source
SCSITaskStatus fCompletionStatus;
```

## Discussion

Use the values that SCSITaskStatus defines to evaluate this field.

## See Also

### Accessing response properties

fServiceResponse

The response from the service, such as complete, in process, or rejected.

fRealizedByteCountOfTransfer

The byte count of the tranferred data.

fSenseDataValid

A Boolean value that indicates whether the sense data that the kernel provides is valid.

