

- SCSIPeripheralsDriverKit
-  READ_CAPACITY 

Function

# READ_CAPACITY

Fills a Command Descriptor Block (CDB) to perform a SCSI read-capacity command.

DriverKit 22.0+

``` source
bool READ_CAPACITY(SCSIDeviceOutParameters * request, UInt64 bufAddr, SCSIDeviceInParameters * response, UInt64 senseBufAddr);
```

## Parameters 

`request`  

An object that contains the request information.

`bufAddr`  

A buffer to receive the data.

`response`  

An empty SCSIDeviceInParameters object. On return, the framework populates this object with the response information.

`senseBufAddr`  

The address of the sense buffer.

## Return Value

`true` if the call successfully fills the CDB; `false`, otherwise.

## Discussion

Use this method in your dext to prefill a 16-byte CDB for the standard `READ CAPACITY` SCSI command.

## See Also

### Creating common SCSI commands

TEST_UNIT_READY

Fills a Command Descriptor Block (CDB) to test whether the unit is ready.

INQUIRY

Fills a Command Descriptor Block (CDB) to perform a SCSI inquiry.

REQUEST_SENSE

Fills a Command Descriptor Block (CDB) to perform a SCSI sense-request command.

READ_10

Fills a Command Descriptor Block (CDB) to perform a SCSI read command.

WRITE_10

Fills a Command Descriptor Block (CDB) to perform a SCSI write command.

