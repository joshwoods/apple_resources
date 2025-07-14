

- Kernel
- Hardware Families
- ATA
-  ATAPIClientData 

Structure

# ATAPIClientData

macOS 11.0+

``` source
typedef struct ATAPIClientData {
    ...
} ATAPIClientData;
```

## Overview

This structure is stuffed into the refcon so we can associate which IOATACommand and SCSITaskIdentifier is completing.

## Topics

### Instance Properties

cmd

IOATACommand for request.

scsiTask

SCSITaskIdentifier of request.

self

Pointer to the object.

## See Also

### ATAPI

IOATAPIProtocolTransport

SCSI Protocol Driver Family for ATAPI Devices.

ATAPICmdPacket

### Related Documentation

