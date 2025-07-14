

- SCSIPeripheralsDriverKit
-  SMART_Write_Log_At_Address 

Function

# SMART_Write_Log_At_Address

Fills a Command Descriptor Block (CDB) to perform a SMART SCSI Command to write log data at an address.

DriverKit 22.0+

``` source
bool SMART_Write_Log_At_Address(SCSIDeviceOutParameters * request, UInt64 bufAddr, UInt8 numSectors, UInt8 logAddress, SCSIDeviceInParameters * response, UInt64 senseBufAddr);
```

## Parameters 

`request`  

An object that contains the request information.

`bufAddr`  

A buffer that holds the data to write.

`numSectors`  

The number of sectors to write.

`logAddress`  

The address of the log.

`response`  

An empty SCSIDeviceInParameters object. On return, the framework populates this object with the response information.

`senseBufAddr`  

The address of the sense buffer.

## Return Value

`true` if the call successfully fills the CDB; `false`, otherwise.

## Discussion

Use this method in your dext to prefill a 16-byte CDB for the standard SMART SCSI Command to write log data at an address.

## See Also

### Creating Self-Monitoring, Analysis and Reporting Technology (SMART) Commands

SMART_Enable_Disable_Operations

Fills a Command Descriptor Block (CDB) to perform a SMART SCSI Command to enable or disable operations.

SMART_Enable_Disable_AutoSave

Fills a Command Descriptor Block (CDB) to perform a SMART SCSI Command to enable or disable the autosave feature.

SMART_Return_Status

Fills a Command Descriptor Block (CDB) to perform a SMART SCSI Command to return status.

SMART_Execute_Offline_Immediate

Fills a Command Descriptor Block (CDB) to perform a SMART SCSI Command to execute an immediate offline test.

SMART_Read_Data

Fills a Command Descriptor Block (CDB) to perform a SMART SCSI Command to read data.

SMART_Read_Data_Thresholds

Fills a Command Descriptor Block (CDB) to perform a SMART SCSI Command to read data thresholds.

SMART_Read_Log_At_Address

Fills a Command Descriptor Block (CDB) to perform a SMART SCSI Command to read log data from an address.

SMART_Get_Identify_Data

Fills a Command Descriptor Block (CDB) to perform a SMART SCSI Command to get identify data.

