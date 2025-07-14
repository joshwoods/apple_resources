

- SCSIPeripheralsDriverKit
-  INQUIRY 

Function

# INQUIRY

Fills a Command Descriptor Block (CDB) to perform a SCSI inquiry.

DriverKit 22.0+

``` source
bool INQUIRY(SCSIDeviceOutParameters * request, UInt64 bufAddr, SCSIDeviceInParameters * response, UInt64 senseBufAddr);
```

## Parameters 

`request`  

An object that contains the request information.

`bufAddr`  

A buffer to receive the inquiry data.

`response`  

An empty SCSIDeviceInParameters object. On return, the framework populates this object with the response information.

`senseBufAddr`  

The address of the sense buffer.

## Return Value

`true` if the call successfully fills the CDB; `false`, otherwise.

## Discussion

Use this method in your dext to prefill a 16-byte CDB for the standard `INQUIRY` SCSI command.

## See Also

### Creating common SCSI commands

TEST_UNIT_READY

Fills a Command Descriptor Block (CDB) to test whether the unit is ready.

REQUEST_SENSE

Fills a Command Descriptor Block (CDB) to perform a SCSI sense-request command.

READ_10

Fills a Command Descriptor Block (CDB) to perform a SCSI read command.

WRITE_10

Fills a Command Descriptor Block (CDB) to perform a SCSI write command.

READ_CAPACITY

Fills a Command Descriptor Block (CDB) to perform a SCSI read-capacity command.

