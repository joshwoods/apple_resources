

- SCSIPeripheralsDriverKit
-  TEST_UNIT_READY 

Function

# TEST_UNIT_READY

Fills a Command Descriptor Block (CDB) to test whether the unit is ready.

DriverKit 22.0+

``` source
bool TEST_UNIT_READY(SCSIDeviceOutParameters * request, SCSIDeviceInParameters * response, UInt64 senseBufAddr);
```

## Parameters 

`request`  

An object that contains the request information.

`response`  

An empty SCSIDeviceInParameters object. On return, the framework populates this object with the response information.

`senseBufAddr`  

The address of the sense buffer.

## Return Value

`true` if the call successfully fills the CDB; `false`, otherwise.

## Discussion

Use this method in your dext to prefill a 16-byte CDB for the standard `TEST UNIT READY` SCSI command.

## See Also

### Creating common SCSI commands

INQUIRY

Fills a Command Descriptor Block (CDB) to perform a SCSI inquiry.

REQUEST_SENSE

Fills a Command Descriptor Block (CDB) to perform a SCSI sense-request command.

READ_10

Fills a Command Descriptor Block (CDB) to perform a SCSI read command.

WRITE_10

Fills a Command Descriptor Block (CDB) to perform a SCSI write command.

READ_CAPACITY

Fills a Command Descriptor Block (CDB) to perform a SCSI read-capacity command.

