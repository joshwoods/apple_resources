

- SCSIPeripheralsDriverKit
- IOUserSCSIPeripheralDeviceType05
-  UserReportMediumBlockSize 

Instance Method

# UserReportMediumBlockSize

Provides a report on the external device’s block size.

DriverKit 22.0+

``` source
kern_return_t UserReportMediumBlockSize(UInt64 * blockSize);
```

## Parameters 

`blockSize`  

On return, the external device’s block size.

## Return Value

A value that indicates the result of the report request. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## Discussion

This call populates `blockSize` with the granularity of the block size, such as 512 bytes or 4096 bytes (4 KB).

