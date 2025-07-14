

- SCSIPeripheralsDriverKit
-  SCSI commands 

API Collection

# SCSI commands

Call the framework’s free functions to populate Command Descriptor Blocks (CDBs) to send to your peripheral.

## Topics

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

READ_CAPACITY

Fills a Command Descriptor Block (CDB) to perform a SCSI read-capacity command.

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

SMART_Write_Log_At_Address

Fills a Command Descriptor Block (CDB) to perform a SMART SCSI Command to write log data at an address.

SMART_Get_Identify_Data

Fills a Command Descriptor Block (CDB) to perform a SMART SCSI Command to get identify data.

### Creating arbitrary SCSI commands

SetCommandCDB

Fills a 16-byte Command Descriptor Block (CDB) with custom content.

### Supporting types

SCSIDeviceOutParameters

A structure that contains parameters for an outbound request to a SCSI device.

SCSIDeviceInParameters

A structure that contains properties from an inbound response from a SCSI device.

