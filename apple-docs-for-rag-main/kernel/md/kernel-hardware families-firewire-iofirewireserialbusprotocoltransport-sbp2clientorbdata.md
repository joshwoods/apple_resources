

- Kernel
- Hardware Families
- FireWire
- IOFireWireSerialBusProtocolTransport
-  SBP2ClientOrbData 

# SBP2ClientOrbData

``` source
typedef struct {
      IOFireWireSBP2ORB *orb;
      SCSITaskIdentifier scsiTask;
      SCSIServiceResponse serviceResponse;
      SCSITaskStatus taskStatus;
      IOBufferMemoryDescriptor *quadletAlignedBuffer;
} SBP2ClientOrbData;
```

## Overview

This structure is stuffed into the refcon so we can associate which IOFireWireSBP2ORB and SCSITaskIdentifier is completing.

