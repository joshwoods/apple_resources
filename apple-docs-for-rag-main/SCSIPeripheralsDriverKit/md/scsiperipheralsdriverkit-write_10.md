

- SCSIPeripheralsDriverKit
-  WRITE_10 

Function

# WRITE_10

Fills a Command Descriptor Block (CDB) to perform a SCSI write command.

DriverKit 22.0+

``` source
bool WRITE_10(SCSIDeviceOutParameters * request, UInt64 blockSize, UInt32 startBlock, UInt16 blockCount, UInt64 bufAddr, SCSIDeviceInParameters * response, UInt64 senseBufAddr);
```

## Parameters 

`request`  

An object that contains the request information.

`blockSize`  

The block size, in bytes, for the data transfer.

`startBlock`  

The Logical Block Address (LBA) of the starting block.

`blockCount`  

The number of blocks to write.

`bufAddr`  

A buffer that holds the data to write.

`response`  

An empty SCSIDeviceInParameters object. On return, the framework populates this object with the response information.

`senseBufAddr`  

The address of the sense buffer.

## Return Value

`true` if the call successfully fills the CDB; `false`, otherwise.

## Discussion

Use this method in your dext to prefill a 16-byte CDB for the standard `WRITE10` SCSI command.

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

READ_CAPACITY

Fills a Command Descriptor Block (CDB) to perform a SCSI read-capacity command.

