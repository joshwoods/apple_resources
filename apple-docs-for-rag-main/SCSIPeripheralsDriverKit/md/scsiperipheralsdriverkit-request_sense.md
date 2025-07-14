

- SCSIPeripheralsDriverKit
-  REQUEST_SENSE 

Function

# REQUEST_SENSE

Fills a Command Descriptor Block (CDB) to perform a SCSI sense-request command.

DriverKit 22.0+

``` source
bool REQUEST_SENSE(SCSIDeviceOutParameters * request, UInt64 bufAddr, UInt8 senseLength, SCSIDeviceInParameters * response);
```

## Parameters 

`request`  

An object that contains the request information.

`bufAddr`  

A buffer to receive the sense-request data.

`senseLength`  

The length of requested sense data, in bytes.

`response`  

An empty SCSIDeviceInParameters object. On return, the framework populates this object with the response information.

## Return Value

`true` if the call successfully fills the CDB; `false`, otherwise.

## Discussion

Use this method in your dext to prefill a 16-byte CDB for the standard `REQUEST SENSE` SCSI command.

## See Also

### Creating common SCSI commands

TEST_UNIT_READY

Fills a Command Descriptor Block (CDB) to test whether the unit is ready.

INQUIRY

Fills a Command Descriptor Block (CDB) to perform a SCSI inquiry.

READ_10

Fills a Command Descriptor Block (CDB) to perform a SCSI read command.

WRITE_10

Fills a Command Descriptor Block (CDB) to perform a SCSI write command.

READ_CAPACITY

Fills a Command Descriptor Block (CDB) to perform a SCSI read-capacity command.

