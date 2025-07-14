

- SCSIPeripheralsDriverKit
- IOUserSCSIPeripheralDeviceType00
-  UserResumeServices 

Instance Method

# UserResumeServices

Resumes normal services after a suspension.

DriverKit 22.0+

``` source
kern_return_t UserResumeServices();
```

## Return Value

A value that indicates the result of the resume request. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## Discussion

Call this method when the dext finishes using its window of exclusivity from a previous UserSuspendServices call so file systems can continue communicating with the drive.

## See Also

### Suspending and resuming services

UserSuspendServices

Suspends services and allows the dext to communicate with the external drive.

