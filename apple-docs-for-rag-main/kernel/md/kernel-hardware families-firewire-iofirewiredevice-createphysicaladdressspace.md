

- Kernel
- Hardware Families
- FireWire
- IOFireWireDevice
-  createPhysicalAddressSpace 

# createPhysicalAddressSpace

Creates local physical FireWire address spaces for the device to access.

``` source
virtual IOFWPhysicalAddressSpace *createPhysicalAddressSpace(
 IOMemoryDescriptor *mem); 
```

## Parameters 

`mem`  

Memory area allocated to back the physical access by Link hardware.

## Return Value

A valid `IOFWPhysicalAddressSpace` object on success; NULL on failure.

## See Also

### Miscellaneous

clearNodeFlags

Resets the node's characteristics.

createPseudoAddressSpace

Creates local pseudo FireWire address spaces for the device to access.

getNodeFlags

Retrieves the node's characteristics.

getUnitCount

Returns number of units attached to this device.

init

Initializes the nub.

setMaxSpeed

Sets the maximum speed for this node.

setNodeFlags

Sets the node's characteristics.

