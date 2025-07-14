

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  UserGetDMASpecification 

Instance Method

# UserGetDMASpecification

Gets the controller-specific direct memory access (DMA) specification in response to a call from the framework.

DriverKit

``` source
kern_return_t UserGetDMASpecification(uint64_t * maxTransferSize, uint32_t * alignment, uint8_t * numAddressBits, DMAOutputSegmentType * segmentType);
```

## Parameters 

`maxTransferSize`  

The maximum allowable transfer size for the controller.

`alignment`  

The required alignment for the controller.

`numAddressBits`  

The number of bits that the hardware uses on its internal address bus.

`segmentType`  

On return, set this output segment type according to the endianness of the hardware.

## Return Value

A value that indicates the result of getting the DMA specification. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## See Also

### Managing Direct Memory Access

DMAOutputSegmentType

The size and endianness that the system uses for direct memory access (DMA).

